
![](https://s1.ax1x.com/2022/05/25/XFqApD.png)

# Oh My Posh 自制主题 —— muxiner

## 自制原因 😶‍🌫️😶‍🌫️😶‍🌫️

Oh My Posh 上有很多优秀的 Themes，可以满足不同人对于不同喜好 Prompt 的需求，可是呢，我前前后后尝试过很多不同的 Theme，但是总感觉不能很好的满足我全部的需求（🥵🥵🥵 颜值上的需求），对是不能满足全部的需求，总有部分的地方符合我的预期（当然也是改变了我对 Prompt 样式的喜好）。

思来想去，总是不得满足，就决定——要不我自制一个自己喜欢的——集很多我喜欢的样式于一体，并修改成自己喜欢的颜色。🙈🙈🙈

> 做决定之前，我也研究过官方主题是如何实现的，就是 json 文件到 视觉界面是如何变化的。就是了解了主题的构成要素。

> 其实这一切 [Oh My Posh | Docs](https://ohmyposh.dev/docs) 上都是有的，也为用户提供了很多的自制的选项。

于是乎，我就照着官方的主题，取其我所爱，去其我所恶，整合为这一我自己很喜欢的 Theme。

## 主题样式

![](https://s1.ax1x.com/2022/05/25/XFbv6J.png)

## 尝试主题

执行命令：
```ps1
oh-my-posh print primary --config 'https://raw.githubusercontent.com/Muxiner/ohmyposh-theme-muxiner/master/muxiner.omp.json' --shell powershell
```

## 使用主题

1. 🦥 下载文件 `muxiner.omp.json`
2. 🦥 找到 `Oh My Posh > Themes` 文件夹
   > 可以使用 everything 工具如图搜索，找到文件夹位置

   ![](https://s1.ax1x.com/2022/05/23/XpkvDg.png)

   > 可能如图所示，显示有多个 Themes 文件夹，这是因为安装多个 Oh My Posh 所致，需仔细审查哪一个文件夹是您需要修改主题的文件夹
3. 🦥 将 `muxiner.omp.json` 移动到上一步所找到的 `Oh My Posh > Themes` 文件夹内
4. 🦥 修改**配置文件**
   + `PowerShell`: 修改 `$PROFILE`
       + 方式一：使用 `scoop install oh-my-posh` 安装的 Oh My Posh
            ```ps1
            oh-my-posh init pwsh --config muxiner.omp.json文件路径 | Invoke-Expression
            ```
       + 方法二：使用 `Install-Module oh-my-posh -Scope CurrentUser -Force` 安装的 Oh My Posh
          ```ps1
            # Set-PoshPromt -Theme <THEME_NAME>
            Set-PoshPromt -Theme muxiner
          ```
5. 🦥 重启终端

## 参考

[Oh My Posh | Docs](https://ohmyposh.dev/docs)
