# ⌨️ GLSL

### OpenGL Shading Language (GLSL)은,

GL 그래픽 라이브러리의 쉐이더 프로그램을 작성하는데 사용 되는 언어이다.

DirectX 의 HLSL, Metal의 MSL 과 대응하는 관계.

### 쉐이더 언어가 필요한 이유

WebGL2 에서 사용되는 언어인, JavaScript, TypeScript 가 아닌 GLSL 을 사용해야만 하는 이유는, 쉐이더 프로그램의 특징과 연관이 있다.

GLSL 을 사용하지 않으면, ARB 어셈블리 언어나 하드웨어 별 언어를 사용해야한다는 불편함이 있다.

쉐이더 언어를 통해, 빌드 타겟 하드웨어에 의존하지 않고, 범용 로직을 작성 할 수 있다.

