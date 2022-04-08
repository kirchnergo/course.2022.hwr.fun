``` ini

BenchmarkDotNet=v0.12.1, OS=macOS 12.3 (21E230) [Darwin 21.4.0]
Intel Core i7-7920HQ CPU 3.10GHz (Kaby Lake), 1 CPU, 8 logical and 4 physical cores
.NET Core SDK=6.0.200
  [Host]     : .NET Core 6.0.2 (CoreCLR 6.0.222.6406, CoreFX 6.0.222.6406), X64 RyuJIT DEBUG
  DefaultJob : .NET Core 6.0.2 (CoreCLR 6.0.222.6406, CoreFX 6.0.222.6406), X64 RyuJIT


```
|   Method |     Mean |     Error |    StdDev |   Median | Ratio | RatioSD |  Gen 0 | Gen 1 | Gen 2 | Allocated |
|--------- |---------:|----------:|----------:|---------:|------:|--------:|-------:|------:|------:|----------:|
| Baseline | 8.058 μs | 0.1562 μs | 0.1535 μs | 8.069 μs |  1.00 |    0.00 | 3.3569 |     - |     - |  13.75 KB |
|     Mine | 5.172 μs | 0.2075 μs | 0.5953 μs | 5.006 μs |  0.57 |    0.02 | 1.8768 |     - |     - |   7.68 KB |
