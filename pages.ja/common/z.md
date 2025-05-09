# z

> 高頻度で利用されるディレクトリを把握し、文字列や正規表現をつかうことでスムーズに移動できるようにします。
> もっと詳しく: <https://github.com/rupa/z>。

- "foo"が名前に含まれるディレクトリに移動する:

`z {{foo}}`

- "foo"と"bar"が名前に含まれるディレクトリに移動する:

`z {{foo}} {{bar}}`

- "foo"と最もマッチングするディレクトリに移動する:

`z -r {{foo}}`

- "foo"とマッチングするディレクトリの中で、最も最近アクセスしたディレクトリに移動する:

`z -t {{foo}}`

- `z`コマンドのデータベースの中で、`foo` にマッチングするディレクトリの一覧を表示する:

`z -l {{foo}}`

- 現在のディレクトリを`z`コマンドのデータベース除去する:

`z -x .`
