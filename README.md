# awesome-solana

## [常用命令](https://www.anchor-lang.com/docs/installation)

安装 Rust 环境

- 安装命令 `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
- 查看版本 `rustc --version`
- 更新最新版本 `rustup update`

Cargo：Rust 的构建工具和包管理器

- 查看版本 `cargo --version`
- 构建项目 `cargo build`
- 运行项目 `cargo run`
- 测试项目 `cargo test`
- 将库发布到 crates.io `cargo publish` _类似 npm 库_

Solana CLI

- 安装命令 `sh -c "$(curl -sSfL https://release.anza.xyz/stable/install)"`
- `export PATH="$HOME/.local/share/solana/install/active_release/bin:$PATH"`
- 查看版本 `solana --version`
- 更新最新版本 `agave-install update`
- 清除缓存 `rm -rf ~/.cache/solana/*`
- 查看当前配置 `solana config get`
- 创建新钱包 `solana-keygen new`
- 查看当前钱包地址 `solana address`
- 获取测试币 `solana airdrop 2`
- 查看钱包持仓情况 `solana balance`
- 切换网络
  - `solana config set -um` # For mainnet-beta
  - `solana config set -ud` # For devnet
  - `solana config set -ul` # For localhost
  - `solana config set -ut` # For testnet

Anchor CLI

- 安装 avm `cargo install --git https://github.com/coral-xyz/anchor avm --force` _类似 nvm 管理版本_
- 查看版本 `avm --version`
- 安装最新版本 `avm install latest`
- 使用最新版本 `avm use latest`
- 查看 Anchor 版本 `anchor --version`

## 教程

- Raydium https://docs.raydium.io/raydium/zhong-wen
- Anchor https://github.com/coral-xyz/anchor
- Solana Web3.js https://solana-labs.github.io/solana-web3.js/
- Solana scan https://solscan.io

## 终端代理

- 全局代理模式
- 查看代理命令 `curl cip.cc`
- 更改代理命令 `export https_proxy=http://127.0.0.1:7897 http_proxy=http://127.0.0.1:7897 all_proxy=socks5://127.0.0.1:7897`
- Noah 视频教程 https://www.bilibili.com/video/BV1Q3cyeTEPJ
