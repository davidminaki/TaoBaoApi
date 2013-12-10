# TaoBaoApi

通过淘宝或天猫商品链接获取商品信息，商品信息包括标题、价格、图片。

## 安装方法

在 Gemfile 文件中加入以下代码:

    gem "TaoBaoApi", "~> 0.0.1"

然后执行:

    $ bundle

或者你可以通过 em installl 直接安装:

    $ gem install TaoBaoApi

## Usage

```ruby

require 'TaoBaoApi'

good = TaoBaoApi::Good.new

info  = good.get_info 'http://item.taobao.com/item.htm?id=16434110195'

p info #hash format,{:title => xxx, :price => xxx, :img => xxx}

```
测试文件见test.rb

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
