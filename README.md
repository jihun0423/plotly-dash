# plotly-dash

인턴을 하며 다른 직원분들의 작업을 보던 도중 시각화가 매우 깔끔하게 정리되어 있었고, 상호작용 가능한 그래프가 그려져 있어서 여쭤봤더니 plotly와 dash를 이용해서 dashboard를 생성한거라고 한다.


평소 시각화 툴이라면 matplotlib이나 가끔 태블로를 사용한 정도라서, 흥미를 가져 공부해 보기로 하였다.  


* 05.09 처음으로 plotly 그래프 작성법을 알게 되었다. 내일은 dash를 이용하여 plotly 그래프를 띄워보고 싶다.  
* 05.10 처음으로 dash를 사용하여 대쉬보드 작성을 할 수 있게 되었다! 다음 목표는 여러개의 그래프를 한 화면에 띄우고, 외부에서 레이아웃을 들여오는 것이다.  
* 05.11 그래프 여러개를 한 화면에 띄우는데 성공하였고, 외부에서 주관적으로 마음에 드는 테마를 불러오는데 성공하였다! 다음 목표는 그래프들의 컬럼을 바꿀 수 있도록 하는 것이다.  
* 05.13 년도별로 슬라이드를 하여 그래프를 보게 하는 기능을 추가 하였다.
* 05.15 하나의 그래프에 컬럼을 원하는 대로 설정하여 바로 반영되도록 하는 것은 성공하였으나, 그래프 여러개를 원하는 대로 변경하는 것은 실패하였다...
* 05.17 드디어 성공하였다!! 어제까지 계속 고민했던 점이, x축 y축을 설정하는 dropdown들을 그래프 위에 각각 2개씩 배치하고 싶었는데, 이상하게도 그렇게만 하면 한 줄에 그래프가 2개씩 있던 것들이 밀려서 그래프가 하나씩 2줄로 나오게 되었다. 이걸 해결한 방법은, 그래프와 드롭다운들을 아예 별개로 설정해주는 것이였다. 드롭다운들을 먼저 배치 해 준뒤, 그 아래에 또 그래프들을 배치하는 식으로 해결하였다. 또한, 이 드롭다운들을 콜백을 이용하여 그래프의 x축, y축을 실시간으로 설정하는 것에 성공하였다!
* 05.18 일정 때문에 시간이 부족하여 조금씩 밖에 수정을 못하였다.. 그래프의 점에 마우스 포인터를 가져다 댔을 때, 더 많은 정보가 담겨 있었으면 좋겠다 생각하여 hover를 통해 추가하였다.
* 05.20 시계열 데이터의 시각화를 해 보았다. 시계열 데이터는 시간별, 일별 월별로 볼때마다 그래프의 특징이 다르게 나타난다고 생각하기 때문에, dropdown을 통해 원하는 기간별 그래프를 볼 수 있도록 하였다. 
