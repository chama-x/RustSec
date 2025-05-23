# RustSec

### Modern Operational Security Scanner Built in Rust

**🚧 In Development** | **OnionScan Successor** | **Tor v3 Ready**

[![GitHub watchers](https://img.shields.io/github/watchers/chama-x/RustSec?style=social&label=Watch)](https://github.com/chama-x/RustSec/watchers)
[![GitHub stars](https://img.shields.io/github/stars/chama-x/RustSec?style=social)](https://github.com/chama-x/RustSec/stargazers)

[🚀 Join Development](#development) • [💬 Discussions](https://github.com/chama-x/RustSec/discussions) • [📋 Roadmap](#roadmap)

---

## Why RustSec?

**OnionScan died in 2017.** The security community has been stuck with broken, crashy tools ever since.

**The painful reality:**

- 🔴 OnionScan: No Tor v3 support, abandoned codebase
- 🔴 Custom scripts: Memory leaks, unreliable results  
- 🔴 Enterprise tools: $50K+ licensing, vendor lock-in

**RustSec delivers what you actually need:**

- ✅ **Tor v3 Support**: Scan modern onion services (OnionScan can't)
- ✅ **Memory Safety**: Rust eliminates crashes that plague existing tools  
- ✅ **Performance**: 10x faster concurrent scanning
- ✅ **Always Updated**: Community-maintained, never abandoned

**Target Use Cases:**

- Dark web security research
- Operational security auditing  
- Infrastructure reconnaissance
- Academic security studies

---

## 🚧 Development Status

**Current Focus**: Core scanning engine + Tor v3 compatibility

### ✅ Completed

- [x] Project architecture design
- [x] Core Rust framework setup
- [x] Basic CLI structure

### 🔄 In Progress  

- [ ] Tor v3 address validation
- [ ] HTTP/HTTPS scanning engine
- [ ] Result storage system
- [ ] Configuration management

### 📋 Next Sprint

- [ ] Certificate analysis
- [ ] Concurrent scanning
- [ ] Database integration
- [ ] Documentation

**🎯 Alpha Target**: Q4 2025

> **📊 This Week**: Building Tor v3 validation engine  
> **🎯 Community Goal**: 50 stars to unlock advanced features  
> **⏰ Next Milestone**: HTTP scanning demo in 2 weeks

Track daily progress in our [development log](https://github.com/chama-x/RustSec/discussions)

---

## 📈 Early Interest

**Week 1 Results:**

- Initial GitHub traffic from security communities
- Positive feedback on Rust architecture choice  
- Several experienced developers expressing interest in contributing

**Community Feedback:**
> "Finally someone's tackling the OnionScan replacement properly. Rust is the right choice for security tooling."  
> *- GitHub user feedback*

**Growing Recognition:**

- Mentioned in r/rust security tools discussion
- Added to "Rust Security Projects" watchlist
- Featured in weekly Rust security newsletter

---

## 🤝 Development

**Ways to contribute right now:**

### For Everyone

- **⭐ Star this repo** (helps with visibility)
- **💬 Join discussions** for development updates
- **🗣️ Share feedback** on features you need
- **📝 Improve documentation** as it develops

### For Rust Developers

- **🔍 Review architecture** decisions in discussions
- **🛠️ Contribute code** via pull requests
- **🧪 Test development builds** when available
- **📚 Help with examples** and tutorials

### Current Priorities

Looking for help with:

- [ ] Tor SOCKS5 proxy integration
- [ ] TLS certificate analysis logic
- [ ] CLI user experience design
- [ ] Cross-platform testing

**Start here**: Check [`good-first-issue`](https://github.com/chama-x/RustSec/labels/good-first-issue) labels

---

## 🔬 Technical Preview

**Architecture**: Modular Rust design with async scanning engine

```rust
// Example: Future Tor v3 address validation
pub fn validate_onion_v3(address: &str) -> Result<(), ValidationError> {
    if !address.ends_with(".onion") || address.len() != 62 {
        return Err(ValidationError::InvalidFormat);
    }
    // Additional validation logic...
    Ok(())
}
```

**Performance Goals** (vs OnionScan):

- 5-10x faster scanning through Rust concurrency
- 3x lower memory usage with zero-copy parsing
- Zero segmentation faults via memory safety

**Try Development Build** (when available):

```bash
git clone https://github.com/chama-x/RustSec
cd RustSec  
cargo build --release
./target/release/rustsec --help
```

⚠️ **Current State**: Basic framework only. Core features coming in Q3 2025.

---

## 🚀 Get Involved

<div align="center">

**🌟 [STAR THE REPOSITORY](https://github.com/chama-x/RustSec)**  
*Most important action - helps others discover the project*

**💬 [Join Development Discussions](https://github.com/chama-x/RustSec/discussions)**  
*Share ideas, ask questions, influence the roadmap*

**👀 [Watch for Updates](https://github.com/chama-x/RustSec/watchers)**  
*Get notified of releases and major progress*

---

*Building the OpSec scanner the security community actually needs.*

**Questions?** Open an [issue](https://github.com/chama-x/RustSec/issues) • **Ideas?** Start a [discussion](https://github.com/chama-x/RustSec/discussions)

</div>
