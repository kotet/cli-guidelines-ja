# Command Line Interface Guidelines (日本語訳)

[cli-guidelines/cli-guidelines](https://github.com/cli-guidelines/cli-guidelines)の日本語訳プロジェクトです。
自由な貢献を受け付けています。

## 翻訳の更新

[Reactの公式ドキュメント等と同じ方式](https://zenn.dev/smikitky/articles/0d250f7367eda9#%E5%8E%9F%E6%96%87%E3%81%B8%E3%81%AE%E8%BF%BD%E5%BE%93)
をとります。
原文をマージし、コンフリクトした状態のままコミットします。
その後、新しい原文をもとに翻訳を行うことでコンフリクトの解消を行います。
新しいパラグラフが追加されている場合はコンフリクトが発生しないため、翻訳漏れのないように注意してください。

```bash
git remote add upstream git@github.com:cli-guidelines/cli-guidelines.git
git fetch upstream
git merge upstream/main
git commit -am "Merge upstream with conflict"
# 翻訳を行う
git commit -am "..."
```

---

# Command Line Interface Guidelines

An open-source guide to help you write better command-line programs, taking traditional UNIX principles and updating them for the modern day.

This is the source code for the guide. To read it, go to [clig.dev](https://clig.dev/).

[Join us on Discord](https://discord.gg/EbAW5rUCkE) if you want to discuss the guide, or just chat about CLI design.

## Contributing

The content of the guide lives in a single Markdown file, [content/_index.md](content/_index.md).
The website is built using [Hugo](https://gohugo.io/).

To run Hugo locally to see your changes, run:

```
$ brew install hugo
$ cd <path>/<to>/cli-guidelines/
$ hugo server
```

To view the site on an external mobile device, run:

```
hugo server --bind 0.0.0.0 --baseURL http://$(hostname -f):1313
```

<!-- TODO: add contact info (how to reach the CLIG creators with questions) -->

## License

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
