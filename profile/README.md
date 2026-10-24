<p align="center">
  <a href="https://plumix.net/?utm_source=github&utm_medium=org_profile&utm_campaign=logo">
    <img src="https://raw.githubusercontent.com/Plumix-Net/Plumix/main/icon.png" width="96" alt="Plumix"/>
  </a>
</p>

<h1 align="center">Plumix</h1>

<p align="center">
  <b>Flutter's widget model, in C#, for every platform .NET reaches.</b><br/>
  <code>Widget</code> → <code>Element</code> → <code>RenderObject</code>, ported faithfully to .NET 10.<br/>
  Desktop, web, Android and iOS from one codebase.
</p>

<p align="center">
  <a href="https://plumix.net/?utm_source=github&utm_medium=org_profile&utm_campaign=hero"><b>🌐 plumix.net</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/Plumix-Net/Plumix">📖 Framework</a>
  &nbsp;·&nbsp;
  <a href="https://www.nuget.org/packages/Plumix/">📦 NuGet</a>
</p>

<p align="center">
  <a href="https://www.nuget.org/packages/Plumix/"><img src="https://img.shields.io/nuget/vpre/Plumix?label=Plumix&logo=nuget" alt="Plumix on NuGet"/></a>
  <a href="https://github.com/Plumix-Net/Plumix/actions/workflows/ci.yml"><img src="https://github.com/Plumix-Net/Plumix/actions/workflows/ci.yml/badge.svg" alt="CI"/></a>
</p>

---

Flutter's architecture — immutable widgets, a reconciled element tree and a
framework-owned render pipeline — has proven itself for complex, fast UIs.
But it's locked to Dart. **Plumix** reimplements that architecture in C#:
the reconciliation loop, the `RenderBox` layout model, the gesture arena,
the navigator, the sliver protocol. Not "Flutter-like" abstractions on top of
another toolkit — the real thing, so porting a Flutter widget to Plumix is a
mechanical translation, not a redesign.

| | |
|---|---|
| 🧬 **Faithful to Flutter** | `StatelessWidget`, `StatefulWidget`, `SetState`, `BuildContext`, `InheritedWidget` behave the way you already know. |
| 🎨 **Material 3 and Cupertino** | `Plumix.Material` brings the M3 component library with full theming; `Plumix.Cupertino` the iOS look. |
| 🖥️📱 **Every platform .NET reaches** | Windows, macOS, Linux, WebAssembly, Android and iOS, with Avalonia as the platform layer (windowing, input, drawing). |
| 🏗️ **Framework-owned rendering** | Layout, paint, compositing, semantics, focus and gestures live in Plumix, not in Avalonia controls. |
| 🧩 **Flutter's package ecosystem** | `provider`, `bloc` and `slang` ported as `Plumix.Provider`, `Plumix.Bloc`, `Plumix.Slang`. |
| λ **C# and F#** | Modern C# on .NET 10, plus `Plumix.FSharp` widget factories and an Elmish (MVU) host. |

```csharp
public sealed class MyApp : StatelessWidget
{
    public override Widget Build(BuildContext context) =>
        new Scaffold(
            body: new Center(
                child: new Text("Hello, Plumix!")));
}
```

```bash
dotnet add package Plumix
dotnet add package Plumix.Material
```

> **Status:** beta. The core framework, rendering, gestures, navigation and
> scrolling are done, and every Material widget family is ported. The
> Cupertino library is in its final stretch, alongside cross-platform
> stability work on the road to the 1.0 API freeze.
> Progress lives in [`CHANGELOG.md`](https://github.com/Plumix-Net/Plumix/blob/main/CHANGELOG.md)
> and [`FRAMEWORK_PLAN.md`](https://github.com/Plumix-Net/Plumix/blob/main/docs/FRAMEWORK_PLAN.md).

---

### 📦 Repositories

| Repo | What it is |
|---|---|
| [**Plumix**](https://github.com/Plumix-Net/Plumix) | The framework: core widgets and render pipeline, Material 3, Cupertino, Android host, F# and Elmish support, samples. On NuGet as `Plumix`, `Plumix.Material`, `Plumix.Cupertino`, `Plumix.Android`. |
| [**Plumix.Packages**](https://github.com/Plumix-Net/Plumix.Packages) | Ports of popular Flutter packages: `Plumix.Provider`, `Plumix.Bloc`, `Plumix.Slang`. |
| [**NetBench**](https://github.com/Plumix-Net/NetBench) | A real-world showcase: an HTTP load-testing tool (like `k6` / `wrk`) with Avalonia on desktop and Plumix on mobile, over a zero-allocation engine. |

### 🤝 Get involved

- ⭐ **Star [Plumix](https://github.com/Plumix-Net/Plumix)** to follow the road to 1.0
- 🐛 **Found a bug or a missing widget?** Open an [issue](https://github.com/Plumix-Net/Plumix/issues)
- 🛠️ **Want to contribute code?** Read [`CONTRIBUTING.md`](https://github.com/Plumix-Net/Plumix/blob/main/CONTRIBUTING.md): Plumix is built AI-first, with Flutter's Dart source as the spec
- 📣 **Know a Flutter developer curious about .NET?** Send them to [plumix.net](https://plumix.net/?utm_source=github&utm_medium=org_profile&utm_campaign=share)

---

<details>
<summary>🇷🇺 По-русски</summary>

<br/>

**Plumix** — UI-фреймворк для .NET с архитектурой Flutter: те же `Widget`,
`Element` и `RenderObject`, тот же жизненный цикл, только на C# (и F#).
Виджет из Flutter переносится на Plumix построчно, без переосмысления.
Material 3 и Cupertino, порты `provider`, `bloc` и `slang`. Работает на
Windows, macOS, Linux, в браузере (WebAssembly), на Android и iOS — Avalonia
даёт окна, ввод и отрисовку, всё остальное фреймворк делает сам.

Сейчас бета: ядро, рендеринг, жесты, навигация, скролл и весь Material готовы,
Cupertino на финишной прямой. Баги и пожелания —
в [issues](https://github.com/Plumix-Net/Plumix/issues).

**[Подробнее → plumix.net](https://plumix.net/?utm_source=github&utm_medium=org_profile&utm_campaign=ru)**

</details>
