# 쉬운 AI (웹 버전)

AI에게 역할을 정해 주고 쉽게 대화하는 웹 앱입니다. `index.html` 파일 하나로 동작합니다.

## 쓰는 방법

- `index.html`을 브라우저(Chrome, Edge 권장)로 열거나, GitHub Pages 같은 곳에 올려서 엽니다.
- 처음 열면 **브라우저 안의 AI**가 기본으로 골라져 있습니다. 가운데 **AI 준비하기**를 누르면, 설치나 키 없이 바로 실습할 수 있습니다 (처음 한 번 AI 파일을 받는 데 몇 분 걸립니다).
- 다른 AI를 쓰려면 왼쪽 **AI 연결**에서 고릅니다.
  - **브라우저 안의 AI (기본)**: 설치도 키도 필요 없습니다. Chrome, Edge 같은 WebGPU 지원 브라우저가 필요합니다.
  - **내 컴퓨터의 Ollama**: 무료. PC에 [Ollama](https://ollama.com/download)가 설치되어 있어야 합니다.
  - **Claude**: Anthropic API 키가 필요합니다.
  - **OpenAI 호환 서비스**: OpenAI, OpenRouter, Groq, LM Studio 등. 주소와 키를 넣습니다.

## Ollama를 웹에서 쓰려면

인터넷 주소에서 내 PC의 Ollama를 부르려면 한 번 설정이 필요합니다.

- Windows: 명령 프롬프트에서 `setx OLLAMA_ORIGINS "*"` 실행
- macOS: 터미널에서 `launchctl setenv OLLAMA_ORIGINS "*"` 실행
- 그다음 Ollama를 완전히 종료했다가 다시 켭니다.

`"*"`는 모든 웹사이트를 허용합니다. 이 페이지 주소만 허용하려면 `"*"` 대신 그 주소를 넣으세요.

## 개인정보

- 대화 내용과 설정은 이 브라우저(localStorage)에만 저장됩니다.
- API 키는 이 브라우저에만 저장되고, 고른 AI 서비스로만 보내집니다. 공용 PC에서는 다 쓴 뒤 **지우기**를 눌러 주세요.
