# Helm Charts

简化开发环境搭建

```bash
helm repo add jiangtj https://jiangtj.github.io/helm-charts
```

## traefik

安装 traefik

```bash
helm repo add traefik https://traefik.github.io/charts
helm repo update
helm install traefik traefik/traefik
```

## hello

```
helm install hello jiangtj/hello
```

visit http://localhost/hello

## nacos

安装 nacos

```bash
git clone https://github.com/nacos-group/nacos-k8s.git
cd operator
helm install nacos-operator ./chart/nacos-operator 
helm install nacos jiangtj/nacos-simple
```