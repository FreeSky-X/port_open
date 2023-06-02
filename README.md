# port_open

Get the open status of an ipv4 port

## Usage

Add this to your Cargo.toml

```
[dependencies]
port_open="0.1.0"
```

## Examples

```
use port_open::get_port_isopen;
fn main() {
  let result = get_port_isopen(&[127, 0, 0, 1], &[80, 5037, 22]);
  for port in result {
      println!("{:?}", res);
  }
}
```

print-out:
PortOpen { ip: 127.0.0.1, port: 80, is_open: false }
PortOpen { ip: 127.0.0.1, port: 5037, is_open: true }
PortOpen { ip: 127.0.0.1, port: 22, is_open: false }

## License

MIT
