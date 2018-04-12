尝试写一个包，了解一下composer，并且尝试上传到github上面,以及使用
    composer require luanguang/try-make
####使用composer进行初始化操作，也就是composer init 如下composer.json
    {
        "name": "luanguang/try-make",
        "description": "try make a package",
        "type": "library",
        "license": "MIT",
        "authors": [
            {
                "name": "Luan Guang",
                //邮箱
            }
        ],
        "minimum-stability": "dev",//这条很重要，因为是开发包，所以这个要定义，不然完成包之后你是无法安装的。
        "require": {
            "php": ">=7.0"
        },
        "autoload": {
            "psr-4": {
                "Flower\\Rose\\": "src/Flower/Rose",
                "Flower\\Lily\\": "src/Flower/Lily"
            }
        }
    }
####根据上面设置的路径，进行添加文件夹。
####在文件夹当中添加php文件，写方法，提交到git上
####到package.org，提交自己git上面的包路径，完成后到本地进行测试
