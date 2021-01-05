``` ini

BenchmarkDotNet=v0.12.1, OS=Windows 10.0.19042
Intel Core i5-8265U CPU 1.60GHz (Whiskey Lake), 1 CPU, 8 logical and 4 physical cores
.NET Core SDK=5.0.101
  [Host]     : .NET Core 5.0.1 (CoreCLR 5.0.120.57516, CoreFX 5.0.120.57516), X64 RyuJIT
  DefaultJob : .NET Core 5.0.1 (CoreCLR 5.0.120.57516, CoreFX 5.0.120.57516), X64 RyuJIT


```
|              Method |     Mean |    Error |    StdDev | Ratio | RatioSD | Rank |  Gen 0 | Gen 1 | Gen 2 | Allocated |
|-------------------- |---------:|---------:|----------:|------:|--------:|-----:|-------:|------:|------:|----------:|
|    GetYearFromSplit | 121.2 ns |  5.72 ns |  16.76 ns |  0.16 |    0.03 |    1 | 0.0508 |     - |     - |     160 B |
| GetYearFromDateTime | 783.1 ns | 39.07 ns | 115.19 ns |  1.00 |    0.00 |    2 |      - |     - |     - |         - |
