# Kubernetes 入門（三）：維運與安全

Kubernetes Beginners 03 — Operations, Security & Monitoring

本專案提供 Kubernetes 入門課程的實作環境與範例，協助初學者了解部署後常見的維運問題、RBAC 權限控制及監控工具。

## 課程內容

### 1. 日常維運（Troubleshooting）
- Deployment / Pod 狀態檢查
- ImagePullBackOff、CrashLoopBackOff
- CPU / Memory Requests 與 Limits
- OOMKilled 故障排除

### 2. 安全界線（RBAC）
- Role、ClusterRole、RoleBinding
- Human User 與 Namespace 權限隔離
- ServiceAccount、Token 與最小權限

### 3. 監控狀態（Metrics）
- Metrics Server 與 kubectl top
- Prometheus
- kube-state-metrics
- Grafana Dashboard

## DEMO 環境

- Oracle Kubernetes Engine（OKE）
- Kubernetes
- Helm
- Prometheus / Grafana

各元件版本及部署方式以專案中的 Helm Values 與安裝紀錄為準。

## Namespace

| Namespace | 用途 |
|---|---|
| kube-system | Kubernetes 系統元件及 Metrics Server |
| monitoring | Prometheus、Grafana |
| k8s-demo | Troubleshooting DEMO |
| team-a / team-b | RBAC 權限隔離 DEMO（規劃中） |

## 安全注意事項

本專案僅供教學與實驗用途。

請勿將 OCI API Key、kubeconfig、私鑰、Token、密碼或其他敏感資訊提交至 Git Repository。

請勿直接將 DEMO 設定套用至正式生產環境。

## 參考資料

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Kubernetes RBAC](https://kubernetes.io/docs/reference/access-authn-authz/rbac/)
- [Prometheus Documentation](https://prometheus.io/docs/)
- [Grafana Documentation](https://grafana.com/docs/)

## License

授權�This project is licensed under the MIT License.
See [LICENSE](LICENSE) for details.
