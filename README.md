# 说明

## 输入建议

将测试用例作命令行运行的参数传递，如生成的main.exe

```bash
./main.exe test_shell.txt
```

## 输出建议

不要换行！

不要换行！

不要换行！

严格按照实验指导书的样式

## 具体用例

### 0.txt

#### 输入

```
cr x 1
cr p 1
cr q 1
cr r 1
to
req R2 1
to
req R3 3
to
req R4 3
to
to
req R3 1
req R4 2
req R2 2
to
de q
to
to
```

#### 输出

```
init x x x x p p q q r r x p q r x x x p x 
```

### 1.txt

#### 输入

```
cr A 1
cr B 1
cr C 1
to
cr D 1
cr E 1
to
cr F 1
req R1 1
req R2 2
to
req R2 1
req R3 3
to
req R4 4
to
req R3 2
to
rel R2 1
to
rel R3 2
to
to
req R3 3
de B
to
to
to
```

#### 输出

```
init A A A B B B C C C C A D D E E B F C C D D E F A A C F A 
```

### 2.txt

#### 输入

```
cr A 1
cr B 1
cr C 1
req R1 1
to
cr D 1
req R2 2
cr E 2
req R2 1
to
to
to
rel R2 1
de B
to
to
```

#### 输出

```
init A A A A B B B E C A D B E C A C 
```

### 3.txt

#### 输入

```
cr A 1
cr B 1
cr C 1
to
cr D 1
cr E 1
cr F 1
to
to
to
req R1 1
req R2 1
to
req R2 1
to
req R3 3
req R4 3
req R4 3
to
req R1 1
cr G 2
req R1 1
de B
req R3 2
cr H 2
cr I 2
to
req R3 3
req R3 2
rel R3 1
to
```

#### 输出

```
init A A A B B B B C A D D D E E F F F B C A G D A A H H I H C C A 
```

### 4.txt

#### 输入

```
cr x 1
cr p 1
cr q 1
cr r 1
to
to
to
req R1 1
to
req R2 1
to
req R3 2
to
to
rel R1 1
to
req R3 3
de p
to
```

#### 输出

```
init x x x x p q r r x x p p q r r x p q r
```

## 贡献

- 0 实验指导书
- 1、2 万志文
- 3 李逢君
- 4 黄晔熙

