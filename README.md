# 🚀 DevOps Batch Custom Resource

## 📄 Overview

Yeh project **Kubernetes Custom Resource Definition (CRD)** use karta hai jisse hum **DevOps training batches** ko Kubernetes cluster ke andar manage kar saken.

Yeh custom resource, **`DevOpsBatch`**, aapko ek single object mein batch ki saari details (jaise naam, duration, mode, aur platform) define karne ki facility deta hai.

---

## 💡 Prerequisites (Kya-kya Chahiye)

Is resource ko deploy aur use karne ke liye, aapke paas yeh hona zaroori hai:

1.  **Kubernetes Cluster** (v1.16+ recommended).
2.  **`kubectl`** tool installed aur cluster se connected.
3. After that deploy this devops-crd.yml file

- Deploy Command:
bash
```
kubectl apply -f devops-crd.yaml

```
- check the crd is create or not 
```
kubectl get devops-crd 
```
- now time to rum cr file for devops-cr
```
kubectl apply -f devops-cr.yaml
```
📝 Usage (Isko Istemal Kaise Karein)
DevOpsBatch objects ko aap standard kubectl commands se manage kar sakte hain.

## Custom Resource Dekhna
Aap kind (DevOpsBatch), plural (devopsbatches), ya shortNames (practice ya junoon) use kar sakte hain:
# Using plural name
bash
```
kubectl get devopsbatches 
```
# Using short name 'junoon'
```
kubectl get junoon 
```
# Getting full YAML of the sample object
bash
```
kubectl get devopsbatch devopsbatch-sample -o yaml
```
1. The file is making for guid only not as preference not this is used only for guid and at the end if 
you have seen any mistake please try to give us akeonledgement to us

---

