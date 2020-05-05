# open-seoul-subway
A refined set of Seoul subway data 

수도권 전철역간 소요시간 및 역들의 정보를 조금 더 쓰기 쉽게 정제 해 놓은 dataset입니다.

## How to use

현재는 역간 소요시간 계산을 위한 matrix만 올려두었습니다. (나머지는 작업중)

travel_time_matrix.csv를 읽어서 메모리에 올려놓으시고, 인덱싱하여 사용하시면 됩니다.

matrix에서 사용할 각 역의 index는 station_code.csv의 첫 번째 field입니다.

```
0,227,227,낙성대
...
51,312,322,불광
```
예를 들어, 낙성대에서 불광역까지의 소요시간이 궁금하다면 matrix의 [0,51] 혹은 [51,0]의 값을 사용하면 됩니다. (단위는 분 입니다.)

참고로, 현 dataset은 경춘선, 경의중앙선, 경부선, 경인선, 서울 1-9호선 및 공항철도만 커버하고 있습니다. (우이경전철, 용인경전철 등은 추후 반영 예정)

### References

- Time tables of National Railway (국철) : [Link](http://www.letskorail.com/ebizcom/cs/guide/guide/guide11.do)
- Time tables of Seoul Metro Line 1 to 8 : [Link](http://www.seoulmetro.co.kr/kr/board.do?menuIdx=546&bbsIdx=2209228)
- Seoul Metro transfer stations : [Link](http://www.seoulmetro.co.kr/kr/board.do?menuIdx=551&bbsIdx=2208455)
- Seoul Metro Station Code Map : [Link](https://data.seoul.go.kr/dataList/OA-15442/S/1/datasetView.do)
- Seoul Metro Station Locations : [Link](https://data.seoul.go.kr/dataList/OA-118/S/1/datasetView.do) 
