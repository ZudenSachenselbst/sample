
# 二分探索：Dev Basics／Keyword - ＠IT https://atmarkit.itmedia.cojp/ait/articles/1704/18/news021.html

<img src="https://image.itmedia.co.jp/ait/articles/1704/18/dt-02.gif" width=400>


# 定番アルゴリズム：線形探索法と二分探索法 | IT企画研究所 https://www.howisit.jp/2017/03/19/linear-and-binary-search/#section311

<img src="https://www.howisit.jp/myblog/wp-content/uploads/2021/11/1fa5c248b7fa2510e6c97a1ed4210eac.jpg" width=400>


# 降順の場合

Binary search https://www.programming-algorithms.net/article/40119/Binary-search


java - Use a Binary Search on an int array sorted in descending order - Stack Overflow https://stackoverflow.com/questions/28283693/use-a-binary-search-on-an-int-array-sorted-in-descending-order


```
#include <stdio.h>

void main(void){
	
	int d[8] = {9,7,6,4,3,2,1};
	
	int min, mid, max, srch, hit;
	
	min = 0;	// initial search left boundary
	max = 7;	// initial search right boundary 
	srch = 6;	// item to find
	hit = -1; 	// candidate index
	
	for(; hit != srch && min < max ; ){
		mid = (min + max) /2;
		hit = d[mid];
		if(         hit == srch ){{
			
		}
		} else if ( hit  < srch) {
			max --;
		} else {  // hit > srch
			min --;
		}
	}	
	
	if( hit == srch ){
		printf("found %d  at d[%d]\n", srch, mid );
	} else {
		printf("%d not found in d", srch);
	}
		
}



```

# online C compiler
Online C compiler and IDE - API provided by Sphere Engine - Ideone.com https://ideone.com/l/c


# 練習問題

```
■問題１
         
     0   1   2   3   4   5   6   7   8        
   +---+---+---+---+---+---+---+---+---+  
 d | 1 | 3 | 5 | 7 | 9 | 11| 13| 15| 17|  
   +---+---+---+---+---+---+---+---+---+  

●上記配列で 3 を探す場合の、 i, min , max, res の値の変化をトレースしてください

   +-------+------+-------+-------+  
   |   i   | min  |  max  |  res  |  
   +-------+------+-------+-------+  
   |  0    |      |       |       |  
   +-------+------+-------+-------+  
   |  1    |      |       |       |  
   +-------+------+-------+-------+  
   |  2    |      |       |       |  
   +-------+------+-------+-------+  
   |  3    |      |       |       |  
   +-------+------+-------+-------+  
   |  4    |      |       |       |  
   +-------+------+-------+-------+  

●上記配列で 4 を探す場合の、 i, min , max, res の値の変化をトレースしてください



   +-------+------+-------+-------+  
   |   i   | min  |  max  |  res  |  
   +-------+------+-------+-------+  
   |  0    |      |       |       |  
   +-------+------+-------+-------+  
   |  1    |      |       |       |  
   +-------+------+-------+-------+  
   |  2    |      |       |       |  
   +-------+------+-------+-------+  
   |  3    |      |       |       |  
   +-------+------+-------+-------+  
   |  4    |      |       |       |  
   +-------+------+-------+-------+  





















■問題２


     0   1   2   3   4   5   6   7   8   9    
   +---+---+---+---+---+---+---+---+---+---+  
 d | 1 | 3 | 5 | 7 | 9 | 11| 13| 15| 17| 19|  
   +---+---+---+---+---+---+---+---+---+---+  

●上記配列で 3 を探す場合の、 i, min , max, res の値の変化をトレースしてください


   +-------+------+-------+-------+  
   |   i   | min  |  max  |  res  |  
   +-------+------+-------+-------+  
   |  0    |      |       |       |  
   +-------+------+-------+-------+  
   |  1    |      |       |       |  
   +-------+------+-------+-------+  
   |  2    |      |       |       |  
   +-------+------+-------+-------+  
   |  3    |      |       |       |  
   +-------+------+-------+-------+  
   |  4    |      |       |       |  
   +-------+------+-------+-------+  


●上記配列で 4 を探す場合の、 i, min , max, res の値の変化をトレースしてください



   +-------+------+-------+-------+  
   |   i   | min  |  max  |  res  |  
   +-------+------+-------+-------+  
   |  0    |      |       |       |  
   +-------+------+-------+-------+  
   |  1    |      |       |       |  
   +-------+------+-------+-------+  
   |  2    |      |       |       |  
   +-------+------+-------+-------+  
   |  3    |      |       |       |  
   +-------+------+-------+-------+  
   |  4    |      |       |       |  
   +-------+------+-------+-------+  





```


