# セットアップ TODO

## Gemfileを整理
1. コメント削除
1. 任意のgemを使うか決める
1. gem定義の並び替え

## bootstrapの設定
https://github.com/twbs/bootstrap-rubygem

## font-awesome-railsの設定
https://github.com/bokmann/font-awesome-rails

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
