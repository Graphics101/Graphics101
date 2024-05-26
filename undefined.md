# 🐋 사용하는 그래픽스 라이브러리와 선정 이유

2024년 현 시점, 브라우저에서 GPU를 활용한 렌더링을 구현할 수 있는 방법은 총 두가지(WebGL, WebGPU)가 제공됩니다.&#x20;

그 중, WebGPU 가 WebGL 과 달리 [Stateless](https://developer.chrome.com/blog/from-webgl-to-webgpu?hl=ko#global\_state) 한 구조를 가지고 있지만, 아직 정식 기술이 아닌, [실험적 단계](https://developer.mozilla.org/en-US/docs/Web/API/WebGPU\_API)라는 단점을 가지고 있습니다.

또한, 비교적 최신 기술이지라 관련 자료나 예제의 양이 WebGL 에 비해 비교적 적다는 점이 러닝 커브를 올리는 요인이라 판단하였습니다.

OpenGL 은 역사가 오래된 낡은 기술이라 이야기 할 수 있지만, 반대로 오랫동안 사용되며 검증된, 그래픽스 라이브러리의 좋은 레퍼런스라고 말 할 수 있습니다.

따라서, 이 문서에서 사용하는 그래픽스 라이브러리는 WebGL 의 최신버전이 WebGL2 를 사용하기로 결정하였습니다.

[WebGL2 는 OpenGL ES 3.0 의 웹 포팅 버전](https://registry.khronos.org/webgl/specs/latest/2.0/#1.1)이므로, 대부분의 내용이 두 라이브러리간에 호환 가능합니다.

따라서, 참고 자료나 사용하는 예시에서 두 라이브러리를 구분치 않고 사용합니다.
