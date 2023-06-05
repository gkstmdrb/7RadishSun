# 7RadishSun
### 문제
![image](https://github.com/gkstmdrb/7RadishSun/assets/114748816/56782e22-d3ad-44de-8cfc-3f68b74b277d)
<br><br>

### 분석

### 설계
1. int N을 입력받아 N개의 배열방을 생성한다.
2. 각 배열방에 무작위 Double형태의 숫자들을 N번 입력받는다.
3. 배열방의 값들을 정렬하여 소숫점 3째자리까지만 출력한다.
<br><br>
### 구현
``` java
import java.util.Arrays;
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class Main {
    public static void main(String[] args) throws IOException{
    	BufferedReader br = new BufferedReader(new InputStreamReader(System.in));


    	int N = Integer.parseInt(br.readLine());
    	
    	double []gr = new double[N];
    	
    	for(int i=0; i<N; i++) {
    		 		gr[i] = Double.parseDouble(br.readLine());
    		}
    	
    	Arrays.sort(gr);
    	for(int j=0; j<7; j++) {
    		System.out.printf("%.3f\n", gr[j]);
    		}
    }
}
```
<br><br>
### 출력
![image](https://github.com/gkstmdrb/7RadishSun/assets/114748816/591dd138-f11a-48a3-9965-90055a374cc2)
