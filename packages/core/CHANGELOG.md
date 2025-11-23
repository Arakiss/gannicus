# gannicus

## 0.3.0

### Minor Changes

- 347516e: feat: v0.3.0 - Multiple providers, benchmarks, and production-ready features

  ### Added

  - **SGLang Provider** - High-performance self-hosted production inference (26k+ tokens/sec, Linux/CUDA)
  - **MLX Provider** - Apple Silicon optimized inference leveraging Metal GPU (macOS M1/M2/M3/M4)
  - **vLLM Provider** - High-performance inference runtime for Linux/CUDA servers (120-160 req/sec)
  - **Hybrid Generation Types** - Type definitions for cost-effective massive dataset generation (Seed + Expand, Multi-Tenant, Time-Series)
  - **End-to-End Tests** - Comprehensive E2E tests for all providers
  - **Benchmark Suite** - Provider comparison and quick test scripts with automatic server management
  - **Production Examples** - Complete examples for SGLang, MLX, and vLLM
  - **Multi-Provider Comparison** - Example demonstrating all providers side-by-side
  - **Benchmark Documentation** - Complete guide for running benchmarks
  - **macOS Inference Runtimes Documentation** - Guide for Apple Silicon users

  ### Changed

  - Updated provider support to include SGLang, MLX, and vLLM
  - Enhanced generator to support multiple providers seamlessly
  - Improved error handling with timeouts (60-120s) and better error messages
  - Optimized batch sizes per provider (SGLang: 50, MLX: 30, vLLM: 50, Ollama: 5)
  - Updated README with comprehensive provider documentation and examples
  - Enhanced provider health checks with better model matching

  ### Fixed

  - Provider availability detection across all platforms
  - Model health checks for all providers with flexible matching
  - Cross-platform compatibility (macOS, Linux, Windows with WSL2)
  - Timeout handling to prevent hanging requests
  - Error message truncation for better readability

## 0.3.0

### Minor Changes

- feat: v0.3 - Multiple providers, benchmarks, and production-ready features

  ### Added

  - **SGLang Provider** - High-performance self-hosted production inference (26k+ tokens/sec, Linux/CUDA)
  - **MLX Provider** - Apple Silicon optimized inference leveraging Metal GPU (macOS M1/M2/M3/M4)
  - **vLLM Provider** - High-performance inference runtime for Linux/CUDA servers (120-160 req/sec)
  - **Hybrid Generation Types** - Type definitions for cost-effective massive dataset generation (Seed + Expand, Multi-Tenant, Time-Series)
  - **End-to-End Tests** - Comprehensive E2E tests for all providers
  - **Benchmark Suite** - Provider comparison and quick test scripts with automatic server management
  - **Production Examples** - Complete examples for SGLang, MLX, and vLLM
  - **Multi-Provider Comparison** - Example demonstrating all providers side-by-side
  - **Benchmark Documentation** - Complete guide for running benchmarks
  - **macOS Inference Runtimes Documentation** - Guide for Apple Silicon users

  ### Changed

  - Updated provider support to include SGLang, MLX, and vLLM
  - Enhanced generator to support multiple providers seamlessly
  - Improved error handling with timeouts (60-120s) and better error messages
  - Optimized batch sizes per provider (SGLang: 50, MLX: 30, vLLM: 50, Ollama: 5)
  - Updated README with comprehensive provider documentation and examples
  - Enhanced provider health checks with better model matching

  ### Fixed

  - Provider availability detection across all platforms
  - Model health checks for all providers with flexible matching
  - Cross-platform compatibility (macOS, Linux, Windows with WSL2)
  - Timeout handling to prevent hanging requests
  - Error message truncation for better readability

### Patch Changes

- 69c2251: fix(cli): resolve type mismatches in generate command and cleanup core logic

## 0.2.1

### Patch Changes

- de992f8: Fix error handling in OllamaProvider and update README with correct model recommendations

  - Add proper error handling when no model is found or configured
  - Fix TypeScript errors (GenerationContext import, ModelTemperature type)
  - Export model utilities from core package
  - Update README.md with correct model names (llama3.2:3b, qwen2.5:7b, llama3.1:8b)
