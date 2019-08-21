オライリー書籍[Pythonで始める機械学習](https://www.oreilly.co.jp/books/9784873117980/)の学習メモ

# Google Colabで実行する上で詰まったところ
## 1章
### `mglearn` の `import` でエラーになる

Colab上でも`!pip`を使うことで`pipコマンド`を実行できる。

```Notebook
!pip install mglearn
```

#### 参考
- [Importing a library that is not in Colaboratory](https://colab.research.google.com/notebooks/snippets/importing_libraries.ipynb)

### `pd.scatter_matrix` が無い
`pd.scatter_matrix`は廃止されたっぽいので、`pd.scatter_matrix`の代わりに`pd.plotting.scatter_matrix`を使う。

```Notebook
grr = pd.plotting.scatter_matrix( # ...
```
