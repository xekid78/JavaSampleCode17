# JavaDotPic2DAry
二次元配列を使ったドット絵表示

## 処理
二次元配列のデータを`拡張for`文を使って出力する。

## コード
```
public class Dotpic2dary {

	public static void main(String[] args) {
		int[][] letterA =
           	{{0,0,1,1,0,0},
             	{0,1,0,0,1,0},
             	{1,0,0,0,0,1},
             	{1,1,1,1,1,1},
             	{1,0,0,0,0,1},
             	{1,0,0,0,0,1}};

		for (int[] line : letterA) {
			for (int dot : line) {
				if (dot == 1) {
					System.out.print("#");
				} else {
					System.out.print(" ");
				}
			}
			System.out.println("");
		}

	}

}
```

## 出力結果  
```
  ##  
 #  # 
#    #
######
#    #
#    #
```
  
## 開発環境
| 開発ツール |  |
|:-|:-|
| OS | Windows10 |
| 統合開発環境(IDE) | Eclipse 4.7.0 Oxygen |
| 開発言語 | Java8 |
