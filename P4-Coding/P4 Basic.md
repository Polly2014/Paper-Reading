# P4 Basic
## 1. P4 Types
- Basic Types
- Header Types
- Typedef
- Struct
- Header Stack
- Header Union
## 2. P4 Parser
- 作用
  - Pakcets => [headers, metadata]
- 格式
  ```c
  state start{
    transition parse_ethernet;
  }
  state parse_ethernet{
    //...
  }
  ```
## 3. P4 Control
- 格式
  ```c
  control MyIngress(){
    /* Daclarations region */
    apply{
      /* Control Flow */
    }
  }
  ```
### 3.1 P4 Tables
- 作用
  - Match-Action Pipline最小单元
## 4. P4 Deparser
