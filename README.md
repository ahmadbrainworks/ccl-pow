# Cocol Proof of Work
[![Build Status](https://travis-ci.org/cocol-project/btcpow.svg?branch=master)](https://travis-ci.org/cocol-project/btcpow)
---

Bitcoin style Proof of Work lib written in Crystal

Docs: https://cocol-project.github.io/ccl-pow

## Installation

1. Add the dependency to your `shard.yml`:

```yaml
dependencies:
  btcpow:
    github: cocol-project/ccl-pow
```

2. Run `shards install`

## Usage

```crystal
require "ccl-pow"
```

#### Mining
```crystal
CCL::Pow.mine(difficulty: "1d00ffff", for: "my_block_data")
```

#### Calculate target based on difficulty bits
```crystal
CCL::Pow::Utils.calculate_target(from: "1d00ffff")
```

## Contributing

1. Fork it (<https://github.com/cocol-project/ccl-pow/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Contributors

- [Cristian Șerb](https://github.com/cserb) - creator and maintainer
