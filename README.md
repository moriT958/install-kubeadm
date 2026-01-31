# Install kubeadm

- kubeadm
- containerd
- runc
- cni plugin

## usage

1. `inventory/hosts.yml` でターゲットノードを指定
1. バージョンなどの細かい設定は各 role の defaults で指定する
1. ansible の SSH 接続に使う鍵は `ansible.cfg` で指定する

コマンド実行例

```bash
ansible-playbook playbooks/setup.yml --ask-become-pass
```

## 参考

ここに書いてあることをコード化しました

- [Install containerd](https://github.com/containerd/containerd/blob/main/docs/getting-started.md)
- [Setup containerd](https://kubernetes.io/ja/docs/setup/production-environment/container-runtimes/#containerd)
- [Install kubeadm](https://kubernetes.io/ja/docs/setup/production-environment/tools/kubeadm/install-kubeadm/)
