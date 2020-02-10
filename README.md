# rust-projects

> rust 相对其他语言来说，绝大部分知识没有可迁移的，所以学起来感觉好难。

## 猜大小游戏 (guessing_game)

```bash
szy0syz@DESKTOP-SZY:/mnt/c/git/rust-projects/guessing_game$ cargo run
    Finished dev [unoptimized + debuginfo] target(s) in 0.06s
     Running `target/debug/guessing_game`
Guess the number!
Please input your guess.
50
You guessed: 50
Too small!
Please input your guess.
75
You guessed: 75
Too big!
Please input your guess.
62
You guessed: 62
Too big!
Please input your guess.
59
You guessed: 59
Too big!
Please input your guess.
53
You guessed: 53
You win!
```

## 端口扫描器（port_sniffer_cli）

> cargo run -- -j 2000 127.0.0.1

```bash
ip_sniffer -h
ip_sniffer -j 100 192.168.1.1
ip_sniffer 192.168.1.1
```

```rust
use std::env;

fn main() {
    let args: Vec<String> = env::args().collect();

    for i in &args {
        println!("{}", i);
    }

    println!("{:?}", args);
}
```

```bash
~/git/rust-projects/port_sniffer_cli on  master! ⌚ 10:13:42
$ cargo run -- -j 100
    Finished dev [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/port_sniffer_cli -j 100`
target/debug/port_sniffer_cli
-j
100
["target/debug/port_sniffer_cli", "-j", "100"]
```

## 聊天软件（chat-app）

## 迷你区块链（toy-blockchain-cli）
