# SPIR-V Translation Test Discrepancy Analysis

This repository documents an investigation into SYCL test cases that **pass with the [SPIRV-LLVM-Translator](https://github.com/KhronosGroup/SPIRV-LLVM-Translator)** but **fail with the [SPIR-V Backend](https://github.com/llvm/llvm-project)**.

The focus is specifically on tests from the [intel/llvm SYCL end-to-end test suite](https://github.com/intel/llvm/tree/sycl/sycl/test-e2e).

---

## 📌 Test results

The following test setups were used for comparison:

1. **PVC with SPIRV-LLVM-Translator**  
   - Results logged in: `PVC_spirv_llvm_translator.log`

2. **PVC with SPIR-V Backend (llvm-project)**  
   - Results logged in: `PVC_spirv_backend.log`

## 🧰 Driver and Tool Versions

*To be filled*

| Component            | Version          |
|---------------------|------------------|
| DPC++ Compiler       | `<to be filled>` |

## ▶️ Commands Used
