# 🧪 Kubernetes Lab : StatefulSet with MySQL

This project demonstrates deploying a *MySQL database using a Kubernetes StatefulSet* with:

- 🔐 Secret for secure password management  
- 💾 Persistent Volume Claim (PVC) for data persistence  
- 🌐 Headless Service for stable networking  
- ⚙️ Tolerations for scheduling on tainted nodes  

---

---

## 🚀 Deployment Steps

### 1️⃣ Apply the configuration

bash
kubectl apply -f secets.yaml
kubectl apply -f pvc.yaml
kubectl apply -f StatefulSet.yaml
kubectl apply -f HeadlessService.yaml
2️⃣ Verify resources
kubectl get pods
kubectl get svc
kubectl get pvc
3️⃣ Connect to MySQL
kubectl exec -it mysql-0 -- mysql -uroot -p
Enter your password when prompted.

✅ Sample Output
<img width="823" height="532" alt="Screenshot from 2026-04-19 20-56-56" src="https://github.com/user-attachments/assets/4a715a27-a2f7-4380-b1c4-29d57e85bdda" />


🛠️ Technologies Used
Kubernetes
Docker
MySQL 5.7
