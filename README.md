## 가상현실 환경에서 키워드 및 이미지 기반 LLM을 활용한 작업 지원_RAG 버전

# 연구 목표
해당 링크 참조:https://github.com/piyakks/manufacturing_with_gpt

기존 사전 프롬프트 기반 LLM 작업 지원 개선버전
# 기존 사전 프롬프팅 기법의 한계점
1.프롬프트 길어짐

2.성능 불안정

3.API 이용의 경우 비용 증가

# 개선안

1.CLIP을 통한 이미지 및 텍스트 사전 임베팅으로 DB생성(작업 메뉴얼, 각 단계 별 이미지 및 설명)  

2.FAISS를 이용한 Retrival 검색 (현재 단계 + 다음 단계 총 2개 추출)

3.검색된 결과(이미지 + 설명)를 기반으로 필요한 정보만 선택적으로 프롬프트에 포함

4.LLM 기반 응답 생성
# 전체 구조
<img width="1500" height="1000" alt="image" src="https://github.com/user-attachments/assets/42a497fd-a770-47aa-b1d1-c11dea872e90" />

