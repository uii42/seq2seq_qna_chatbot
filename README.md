# Seq2Seq Q&A Chatbot — README

간단한 규칙 기반이 아닌 신경망 Seq2Seq 모델(Luong Attention)로 한국어 Q→A 대화를 학습·추론하는 프로젝트입니다.
데이터는 공개 한국어 챗봇 데이터셋(약 1.17만 쌍)을 사용하고, SentencePiece로 서브워드 토크나이징을 수행합니다.
노트북(.ipynb)에서 **학습→평가→대화(Chat)**까지 한 번에 실행할 수 있습니다.


project/

├─ data/

│  ├─ ChatbotData.csv              # 학습에 사용된 원본 CSV(자동 저장)

│  ├─ spm_kor_v6b.model/.vocab    # SentencePiece 모델/사전(자동 생성)

│  └─ spm_corpus_v6b.txt          # SPM 학습 코퍼스(자동 생성)

├─ checkpoints_v6b/               # 베스트 가중치 저장 폴더(자동 생성)

│  └─ weights.keras

├─ seq2seq_qna_chatbot_v6b.ipynb  # 메인 노트북(학습/평가/챗봇)

└─ README.md
