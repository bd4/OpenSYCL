if(WITH_LLVM_TO_AMDGPU_AMDHSA)
  libkernel_generate_bitcode_target(
      TARGETNAME amdgpu-amdhsa 
      TRIPLE amdgcn-amd-amdhsa
      SOURCES barrier.cpp core.cpp half.cpp integer.cpp math.cpp native.cpp relational.cpp subgroup.cpp localmem.cpp
      ADDITIONAL_ARGS -nogpulib)
endif()
