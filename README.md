# -0910
def solution(strings, n):
  """
  문자열 리스트를 n번째 문자를 기준으로 정렬합니다.

  Args:
    strings: 문자열로 구성된 리스트
    n: 정렬 기준이 되는 문자열의 인덱스

  Returns:
    정렬된 문자열 리스트
  """
  return sorted(strings, key=lambda x: x[n])

# 입출력 예시
strings1 = ['sun', 'bed', 'car']
n1 = 1
print(f"입력: {strings1}, n: {n1} -> 출력: {solution(strings1, n1)}")
# 결과: ['car', 'bed', 'sun']

strings2 = ['abce', 'abcd', 'cdx']
n2 = 2
print(f"입력: {strings2}, n: {n2} -> 출력: {solution(strings2, n2)}")
# 결과: ['abcd', 'abce', 'cdx']
