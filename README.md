# Build

```
docker build -f Dockerfile-iverilog -t stevenmburns/iverilog .
docker build -f Dockerfile -t stevenmburns/dart-and-iverilog .
```

# Run

```
docker run -it stevenmburns/dart-and-iverilog
```
then in the container:
```
export PATH=/icarus_install/bin:$PATH
git clone https://github.com/stevenmburns/rohd_sklansky
cd rohd_sklansky
dart test
```
