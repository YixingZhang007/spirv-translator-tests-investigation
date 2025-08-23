# SPIR-V Investigation for SYCL E2E Tests

This repository documents an investigation into SYCL end-to-end (E2E) test cases that **pass using [SPIRV-LLVM-Translator](https://github.com/KhronosGroup/SPIRV-LLVM-Translator)** but **fail with the [SPIR-V Backend](https://github.com/llvm/llvm-project)**.

The focus is specifically on tests from the [intel/llvm SYCL end-to-end (E2E) test suite](https://github.com/intel/llvm/tree/sycl/sycl/test-e2e).

---

## 📌 Test Results

The results of SYCL E2E tests under different configurations are summarized below:

| Platform | SPIRV-LLVM-Translator Log | SPIR-V Backend Log | Comparison of Results |
|----------|---------------------------|------------------|---------------------|
| PVC      | `PVC_spirv_llvm_translator.log` | `PVC_spirv_backend.log` | `pvc_test_result_summary.md` |
| DG2      | `DG2_spirv_llvm_translator.log` | `DG2_spirv_backend.log` | `DG2_test_result_summary.md` |
| CPU      | `CPU_spirv_llvm_translator.log` | `CPU_spirv_backend.log` | `CPU_test_result_summary.md` |

---

## 🧰 Driver and Tool Versions

| Component              | Version                                                                                     | Project Link                          |
|------------------------|---------------------------------------------------------------------------------------------|---------------------------------------|
| SYCL                   | Git Commit: `b6a619ec00d740be5c340d447fb1f71cf75d653a`                                      | [intel/llvm -b sycl](https://github.com/intel/llvm) |
| SPIRV-LLVM-Translator  | Default version included in the SYCL repository                                             |                                       |
| SPIR-V Backend         | Default version included in the SYCL repository                                             |                                       |
| Driver (Level Zero)    | `level_zero:gpu` - Intel® oneAPI Unified Runtime over Level-Zero, Max 1550, version `12.60.7 [1.6.34666+3]` | [QuickBuild Link](https://ubit-gfx.intel.com/build/22049244) |

---

