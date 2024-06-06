# 🏮 Graphics pipeline

{% hint style="info" %}
[WebGL2 기초](https://webgl2fundamentals.org/webgl/lessons/ko/webgl-fundamentals.html)  [WebGL state diagram](https://webgl2fundamentals.org/webgl/lessons/resources/webgl-state-diagram.html?exampleId=smallest-glsl#no-help) 의 문서를 참고해 작성되었습니다.
{% endhint %}

그래픽스 라이브러리 또한, 여러 프레임워크 사용경험과 비슷하게,\
그래픽스 API 가 지정한 방식과 순서로 코드를 작성 해야만 동작하는 프로그램을 작성 할 수 있습니다.

이러한 과정을 [**그래픽스 파이프라인** **Graphics pipeline**](https://ko.wikipedia.org/wiki/%EA%B7%B8%EB%9E%98%ED%94%BD%EC%8A%A4\_%ED%8C%8C%EC%9D%B4%ED%94%84%EB%9D%BC%EC%9D%B8) (a.k.a 렌더링 파이프라인) 이라고 부릅니다.

사용하는 그래픽스 라이브러리의 종류와 버전에 따라 이 과정은 확장되거나 축소 될 수 있습니다.

[이 문서에서는 WebGL2, 혹은 OpenGL ES 3.0 의 graphics pipeline 을 기준으로 설명](../undefined.md)합니다.&#x20;

TODO:// 각 단계에 맞는 문서 페이지 작성

1. Vertex Specification
   1. Vertex Rendering
2. Vertex Processing
   1. [Vertex Shader](vertex-shader.md)
   2. Tessellation
   3. Geometry Shader
3. Vertex post-processing
   1. Transform Feedback
   2. Primivice assembly
   3. Clipping
   4. Face culling
4. Rasterization
5. [Fragment Processing](fragment-shader.md)
6. Per-Sample Operations
