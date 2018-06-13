# 第1章　ブートローダーとか

## 書き込むまでの方法
### 必要環境
- gcc-3.4.6 h300-elf
- binutils
- h8write
- make

###手順
#### 1. ソースコードをコンパイルし、ELF形式の実行ファイルを作る。

```bash
% make all
```

#### 2. ELF形式の実行ファイルをモトローラSレコード・フォーマット形式に変換する。

```bash
% make image
```

#### 3. 書き込む(Linuxの場合)

```bash
% make write
```

このとき、環境によってはMakefileのH8WRITE_SERDEVのPATHを変更する必要がある。
