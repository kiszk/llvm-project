set(LLVM_LINK_COMPONENTS
  Core
  IRReader
  OrcJIT
  ExecutionEngine
  Support
  nativecodegen
  Analysis
  Passes
  )

add_llvm_example(ThinLtoJIT
  main.cpp
  ThinLtoJIT.cpp
  ThinLtoModuleIndex.cpp
  ThinLtoInstrumentationLayer.cpp
  ThinLtoDiscoveryThread.cpp
  )
