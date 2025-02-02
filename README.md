# alf-reasoning

Alfred에서 추론할 수 있는 LLM모델의 출력 결과중 reasoning만 추출해내는 workflow 입니다.  
reasoning이 끝난 후에는, API response를 받는 sub process를 kill 하여 출력 요금을 최소화합니다.  
사용가능한 모델은 deepseek-r1와 perplexity sonar reasoning 이며  
deepseek-r1의 경우에는 API사용비용을 최소화하기 위해 DeepSeek와 DeepInfra Provider만 사용하도록 제한했습니다.

코드는 추후 업데이트 하도록 하겠습니다.

## How to use
- alfred에서 "rs" 입력하면 workflow가 나타나며, 엔터를 누릅니다.
- TextView component가 출력되며, 하단에는 프롬프트를 입력할 수 있습니다.
- reasoning(CoT) 생성하기 희망하는 prompt를 입력한 후 엔터를 누릅니다.
- 조금만 기다리면 출력이 시작됩니다. 혹시 실수로 창을 닫더라도, workflow에 재진입하면 여전히 처리중인 것을 확인할 수 있습니다.
- 출력이 완료되면 입력창 아래에 완료되었다는 footer가 출력됩니다.
- 새로운 프롬프트를 입력하고싶다면 cmd + 엔터, 출력된 reasoning을 복사하고싶다면 control + 엔터 를 입력합니다.

## Requirement
- Alfred > 5.5
- python3
- OpenRouter API Key

## Install
release에서 alfred workflow를 다운로드하여 실행합니다.

## Demo
![blank](./imgs/demo.gif)