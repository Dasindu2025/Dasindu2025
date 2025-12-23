export default function App() {
  return (
    <div className="min-h-screen bg-black text-white font-sans overflow-x-hidden">
      {/* Glow background */}
      <div className="fixed inset-0 -z-10">
        <div className="absolute -top-40 -left-40 w-96 h-96 bg-purple-600/30 blur-3xl rounded-full" />
        <div className="absolute top-1/3 -right-40 w-96 h-96 bg-cyan-500/30 blur-3xl rounded-full" />
      </div>

      {/* HERO */}
      <section className="flex flex-col items-center justify-center text-center py-32 px-6">
        <h1 className="text-5xl md:text-7xl font-extrabold tracking-tight">
          Dasindu Sithmira
        </h1>
        <p className="mt-4 text-xl text-cyan-400">
          Hela Dev LK • Performance Tooling • Game Utilities
        </p>
        <p className="mt-6 max-w-2xl text-gray-300">
          Building real Windows performance tools.
          No fake sliders. No magic buttons. Just honest optimization.
        </p>

        <div className="mt-10 flex gap-4 flex-wrap justify-center">
          <a
            href="https://github.com/Dasindu2025"
            className="px-6 py-3 rounded-xl bg-gradient-to-r from-purple-600 to-cyan-500 font-semibold hover:scale-105 transition"
          >
            GitHub
          </a>
          <a
            href="#projects"
            className="px-6 py-3 rounded-xl border border-white/20 hover:bg-white/10 transition"
          >
            Projects
          </a>
        </div>
      </section>

      {/* MAIN PROJECT */}
      <section className="max-w-6xl mx-auto px-6 py-24">
        <h2 className="text-4xl font-bold mb-6">
          PulseBoost™ FPS Optimizer
        </h2>
        <p className="text-gray-300 max-w-3xl mb-10">
          Pro-level gaming optimization, but transparent and reversible.
          A Windows desktop app focused on safe performance tuning.
        </p>

        <div className="grid md:grid-cols-2 gap-6">
          {[
            "C# / .NET 8 / WPF (MVVM)",
            "GX-style dark desktop UI",
            "Safe registry, services & power tweaks",
            "Disk & cache cleanup",
            "Network tuning (safe hints only)",
            "Game presets: Lite / Performance / Competitive",
            "In-game HUD (CPU / RAM / Ping)",
            "Everything reversible by design",
          ].map((item) => (
            <div
              key={item}
              className="p-5 rounded-2xl bg-white/5 border border-white/10 backdrop-blur hover:border-cyan-400/50 transition"
            >
              {item}
            </div>
          ))}
        </div>
      </section>

      {/* TECH STACK */}
      <section className="max-w-6xl mx-auto px-6 py-24">
        <h2 className="text-4xl font-bold mb-10">Tech Stack</h2>
        <div className="flex flex-wrap gap-4">
          {[
            "C#",
            ".NET 8",
            "WPF",
            "Visual Studio",
            "VS Code",
            "GitHub",
            "Unreal Engine",
            "Blender",
          ].map((tech) => (
            <span
              key={tech}
              className="px-5 py-2 rounded-full bg-gradient-to-r from-purple-600/40 to-cyan-500/40 border border-white/10"
            >
              {tech}
            </span>
          ))}
        </div>
      </section>

      {/* PROJECTS */}
      <section id="projects" className="max-w-6xl mx-auto px-6 py-24">
        <h2 className="text-4xl font-bold mb-10">Featured Project</h2>

        <div className="p-8 rounded-3xl bg-white/5 border border-white/10 hover:border-purple-500/50 transition">
          <h3 className="text-2xl font-semibold mb-2">
            Smart Calculator (Python + Tkinter)
          </h3>
          <p className="text-gray-300 mb-4">
            Beginner desktop calculator focused on clean logic and UI basics.
          </p>
          <a
            href="https://github.com/Dasindu2025/smart-calculator"
            className="text-cyan-400 hover:underline"
          >
            View Repository →
          </a>
        </div>
      </section>

      {/* FOOTER */}
      <footer className="py-16 text-center text-gray-400">
        <p>
          “Build real tools. No fake sliders. No magic buttons.”
        </p>
        <p className="mt-2">
          © {new Date().getFullYear()} Dasindu Sithmira
        </p>
      </footer>
    </div>
  );
}
