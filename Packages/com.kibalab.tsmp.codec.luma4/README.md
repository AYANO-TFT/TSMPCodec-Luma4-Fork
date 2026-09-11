# TSMP Codec Luma4

TSMP の標準 codec パッケージです。Luma4 は初回セットアップやストリーム経路の診断に使う基準 codec として推奨されます。

## 要件

- TSMP Core: https://github.com/kibalab/TSMP-Core
- Unity 2022.3
- `com.kibalab.tsmp.core` 0.2.0 以降 (UPM 依存バージョン: 0.2.0)
- VRChat ワールドで使用する場合のみ VRChat Worlds SDK 3.9.0 以降が必要

## 使い方

TSMP Core と一緒にこのパッケージをインストールし、Core の `Samples/TSMPController.prefab` をシーンに配置します。その後、`TSMPSetup` の Codec タブで `Luma4` を選択し、`Apply Setup` を実行します。

通常の Unity では、UPM の **Add package from disk** で Core 0.2.0 とこのパッケージをインストールできます。VRCSDK/UdonSharp は不要です。両環境で同じ Controller プレハブを使い、コンポーネントとバインディングは自動準備されます。

## リリース状態

Luma4 0.0.3 は TSMP Core 0.2.0 向けの正式リリースです。1.0 より前は公開 API が変更される場合があります。
