# Matrix

어떤 행렬이 주어질 때, 그 행렬의 특정 행 혹은 열의 성분들을 출력해 줄 수 있는 클래스를 작성하라.

예를 들어 다음과 같이 세 줄로 숫자들이 주어진다면

    > 9 8 7  
    > 5 3 2  
    > 6 6 7 

이는 아래와 같은 행렬을 나타내는 것이다.

        0  1  2
      |---------
    0 | 9  8  7
    1 | 5  3  2
    2 | 6  6  7

여기에서 1행의 성분은

    5, 3, 2

0열의 성분은

    9, 5, 6

이 될 것이다.

## Structure

Matrix 클래스를 작성한다. 생성자를 통해 행렬을 전달받는다.

행렬은 다음과 같은 문자열의 형태로 전달받는다. 예를 들어

    "1 4 9\n16 25 36"

라면, 다음과 같은 행렬을 의미한다.

        0  1  2
      |---------
    0 | 1  4  9
    1 | 16 25 36

다음 프로퍼티들을 작성한다.

    var rows: [[Int]]

각 행별 성분들의 배열을 반환한다. 예를 들어 위의 행렬의 경우에는 [[1, 4, 9], [16, 25, 35]] 를 반환한다.

    var columns: [[Int]]

각 열별 성분들의 배열을 반환한다. 예를 들어 위의 행렬의 경우에는 [[1, 16], [4, 25], [9, 36]] 을 반환한다.

## Source

    class Matrix {

        var matrix: [[Int]] // save the matrix here

        var rows: [[Int]] {
            get {
                /* write your code here */
            }
        }

        var columns: [[Int]] {
            get {
                /* write your code here */
            }
        }

        init(_ matrix: String) {
            /* write your code here */
        }
    }
