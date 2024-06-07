# 🚿 Vertex Shader

{% hint style="info" %}
[WebGl2 State Diagram(Smallest GLSL)](https://webgl2fundamentals.org/webgl/lessons/resources/webgl-state-diagram.html?exampleId=smallest-glsl) 문서를 [기반으로 설명](../undefined.md)합니다.
{% endhint %}

### 역할

GPU 에서 실행되는 프로그램 입니다.\
정점의 위치와 크기를 정의합니다.

해당 쉐이더에 대한 코드는 [GLSL(OpenGL Shading Language)](../glsl.md) 라는 전용 언어로 작성됩니다.

### Input

Vertex Shader는 외부에서 전달된 각 정점의 위치와 크기, 색상 또는 텍스쳐를 그래픽스 파이프라인의 다음 단계에서 필요한 데이터로 변환합니다. Vertex Shader의 코드는 GPU에서 실행되기 때문에, CPU에서 정의된 데이터를 Vertex Shader에서 사용하려면 특수한 키워드를 사용해야 합니다.

#### in

```glsl
layout(location = 0) in vec3 position;
layout(location = 1) in vec2 texture_coords;
```

`in` 키워드는 **각 정점에 대한 특성을 전달**할 때 사용됩니다. 위의 코드에서는 정점의 위치와 텍스쳐의 좌표만 전달하고 있지만, 정점의 크기나 색상 등 다양한 정보들도 함께 전달할 수 있습니다.

> `layout` 키워드는 무엇인가요?\
> \
> 정보를 **VAO의 특정 위치에 명시적으로 할당**할 때 사용됩니다. 예를 들어, `layout(location = 0)`은 해당 데이터가 VAO의 0번 인덱스에 할당된다는 것을 의미합니다. `layout` 키워드를 생략할 경우, OpenGL에서 위치를 자동으로 할당합니다.

#### uniform

```glsl
uniform mat4 model;
uniform mat4 view;
uniform mat4 projection;
```

`uniform` 키워드는 변하지 않는 데이터를 전달할 때 사용됩니다. 예를 들어 조명, 투영 공간 등 **한 프레임 내에서 모든 정점에 대해 일관된 정보를 제공**해야 할 때 사용할 수 있습니다.
