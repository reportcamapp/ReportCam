# 第三方开源许可声明

**适用版本**：报料相机 ReportCam 0.9.2

本应用使用了下列第三方开源组件。依据 Apache License 2.0 第 4 条及其它相应许可条款，特此声明。
完整许可文本见各组件官方发布页。

> 应用内副本：`app/src/main/res/raw/third_party_notices.txt`
> （用户在「设置 → 关于与声明 → 查看完整许可声明」可离线阅读）。
> 两处须保持一致。

---

## 一、随应用分发的组件（打包进 APK）

| # | 组件 | 坐标 | 许可 |
| --- | --- | --- | --- |
| 1 | AndroidX Core KTX | `androidx.core:core-ktx:1.13.1` | Apache 2.0 |
| 2 | AndroidX AppCompat | `androidx.appcompat:appcompat:1.7.0` | Apache 2.0 |
| 3 | AndroidX Activity KTX | `androidx.activity:activity-ktx:1.9.2` | Apache 2.0 |
| 4 | AndroidX ConstraintLayout | `androidx.constraintlayout:constraintlayout:2.1.4` | Apache 2.0 |
| 5 | AndroidX Lifecycle Runtime | `androidx.lifecycle:lifecycle-runtime-ktx:2.8.6` | Apache 2.0 |
| 6 | CameraX Core | `androidx.camera:camera-core:1.5.3` | Apache 2.0 |
| 7 | CameraX Camera2 | `androidx.camera:camera-camera2:1.5.3` | Apache 2.0 |
| 8 | CameraX Lifecycle | `androidx.camera:camera-lifecycle:1.5.3` | Apache 2.0 |
| 9 | CameraX Video | `androidx.camera:camera-video:1.5.3` | Apache 2.0 |
| 10 | CameraX View | `androidx.camera:camera-view:1.5.3` | Apache 2.0 |
| 11 | CameraX Effects | `androidx.camera:camera-effects:1.5.3` | Apache 2.0 |
| 12 | Material Components for Android | `com.google.android.material:material:1.12.0` | Apache 2.0 |
| 13 | Kotlin Standard Library | `org.jetbrains.kotlin:kotlin-stdlib` | Apache 2.0 |

许可全文：<https://www.apache.org/licenses/LICENSE-2.0>

上述组件均为宽松许可，允许在闭源商业产品中自由使用、修改与再分发，
**不要求衍生作品开源，不具传染性**。

| # | 组件 | 许可 |
| --- | --- | --- |
| 14 | Google Play services 相关组件（CameraX 与 AndroidX 的传递依赖） | Android Software Development Kit License Agreement / Google Play services Terms of Service — <https://developer.android.com/studio/terms> |

---

## 二、仅测试期使用，不打包进 APK

| # | 组件 | 坐标 | 许可 |
| --- | --- | --- | --- |
| 15 | JUnit | `junit:junit:4.13.2` | Eclipse Public License 1.0 — <https://www.eclipse.org/legal/epl-v10.html> |

JUnit 仅在 `testImplementation` 作用域，用于本地 JVM 单元测试，**不会进入发布产物**。

---

## 三、已移除的组件

以下组件曾用于「车牌识别」功能，**已于 v0.9.2 整体移除**：

| 组件 | 坐标 | 许可 |
| --- | --- | --- |
| ML Kit Text Recognition (Chinese) | `com.google.mlkit:text-recognition-chinese:16.0.1` | **ML Kit Terms of Service**（并入 Google APIs Terms of Service），非开源许可证 — <https://developers.google.com/ml-kit/terms> |

**移除原因**：该条款允许 ML Kit 向 Google 回传 API 性能与用量指标，并要求开发者向用户披露这一处理行为，与本应用「无第三方遥测」的定位冲突；同时其端侧模型让 APK 体积从约 6 MB 增加到 31.3 MB。

详见 `docs/compliance-asset-audit.md` R03。

---

## 四、图形素材与字体

- **启动图标与全部界面图形**：本项目自绘矢量图形（Android Vector Drawable / Shape Drawable），未使用任何第三方图标库或素材站资源。
- **字体**：未打包任何字体文件，全部使用 Android 系统字体（含 `monospace`）。

因此本应用在图形素材与字体方面**不存在第三方的署名义务**。

---

## 五、结论

本应用**不包含**任何 GPL / LGPL / AGPL 等具有传染性的许可证组件，
全部运行时依赖均为宽松许可，可安全用于闭源商业分发。
