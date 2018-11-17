# セットアップ TODO

## Gemfileを整理
1. コメント削除
1. 任意のgemを使うか決める
1. gem定義の並び替え

## config/application.rbに以下を追加

```
    config.generators do |g|
      g.test_framework :rspec,
                       view_specs: false,
                       helper_specs: false,
                       routing_specs: false,
                       request_specs: false
    end

    config.i18n.default_locale = :ja
    # Rack Dev Mark
    config.rack_dev_mark.enable = true
```

## Gem設定の確認

以下のURLにアクセスする
html://localhost:3000/samples/index

