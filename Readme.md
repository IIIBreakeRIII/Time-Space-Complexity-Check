## 알고리즘 시, 공간 복잡도 측정기

### 사용 방법

> **Python 가상환경 변경**
개인이 사용하고 있는 Python 가상환경으로 변경합니다.  
이때, `matplotlib` 버전으로 인해, `3.10.x` 이상의 가상환경을 사용하는 것을 권장합니다.  

자세한 내용은, [matplotlib 공식 릴리즈 문서](https://discourse.matplotlib.org/t/matplotlib-announce-ann-matplotlib-3-10-0/25601)를 참고해주세요.  

> `pip install -r requirements.txt`

위의 명령어를 개인이 사용하는 Terminal 에 입력하여 필요 패키지들을 설치합니다.  

> `python measure_complexity.py`
> `python measure_complexity.py --sizes 1000 2000 3000 4000 5000`

위의 두 명령어로 사용이 가능합니다.  
`default sizes = 10000, 20000, 40000, 80000, 160000, 320000`을 사용한다면 첫번째 명령어를,  
사이즈를 조절해서 사용하고 싶다면 `--sizes` 옵션에 원하는 사이즈 5개를 입력해주시면 됩니다(쉼표 구분 없음).  

> `times, mem_mib, mem_kib = measure(eratosthenes, input_sizes)`
`101 lines`에 선언되어 있는 `eratosthenes` 함수는 테스트를 진행하기 위한 함수입니다.  
개인이 확인하고 싶은 알고리즘을 해당 부분에 넣거나, `import` 하신 후에,  
`110 lines`에 선언되어 있는 `times, mem_mib, mem_kib` 부분의 함수 파라미터를 위와 같이 수정합니다.
