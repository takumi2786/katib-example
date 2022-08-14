## 概要
kubeflowのAutoML機能であるkatibを使うためのマニフェスト


## 注意事項
以下のようにサイドカーインジェクションを無効化する必要がある
```yaml
spec:
template:
	metadata:
		annotations: 
		sidecar.istio.io/inject: "false"
```