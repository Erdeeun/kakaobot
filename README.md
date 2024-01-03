# kakaobot
kakao_ai_chatbot
## 카카오톡을 UI로 사용하여 chatbot을 구현했습니다.
1. kakao business로 접속하여 새로운 chatbot 생성
2. chatbot 스킬 추가
   - google colab에서 ngrok 사용
   1) 코드 ngrok으로 실행하는 url 입력 (url/chat/)
   2) 저장 후 배포
      ngrok을 이용하면 다시 실행할 때마다 url이 새로 생성되어 chatbot 스킬과 배포를 여러번 해야하는 번거로움이 있습니다.
   - 구름 ide사용
   1) 구름 ide에서 새로운 컨테이너를 생성
   2) 코드 입력 후 (터미널에서 install 다시 실행, %%writefile... 코드 삭제, terminal에서는 node file과 함께 작동되어 느리게 동작하므로 오른쪽 위에서 kakaobot만 동작하는 터미널을 써도  
      좋습니다, uvicorn kakaobot:app --reload --host=0.0.0.0 --port=80 입력)
   3) 카카오 비지니스 챗봇에 스킬 등록과 배포를 실행합니다.
   4) 구름 ide는 url이 새로 생성되지 않아 새로 배포를 하거나 다시 동작할 때 url을 새로 입력하지 않아도 되는 편리함이 있습니다. 그러나 무료버전을 이용한다면 실행 후 사용하지 않을 때 실행 
      중지를 꼭 해야 합니다. 또한 6개월이 지나도록 다시 실행하지 않으면 컨테이너가 삭제됩니다.)
3. kakao business 채널로 접속하여 홍보하기 url로 들어가면 chatbot과 대화할 수 있는 스티커가 있습니다.
4. 코드에 쓰여 있는대로 이미지를 원한다면 '/img 내용' 방식의 프롬프트를 작성하고 질문에 대한 답을 원한다면 '/ask 내용' 방식의 프롬프트를 작성하십시오
5. chatbot과 대화하며 원하는 정보를 얻고 즐거운 시간을 보내세요!
      
