### Build the image

<blockcode>docker-compose up -d --build</blockcode>

### Build with Persistent Storage

Check for storage
<blockquote>
kubectl get sc
</blockquote>

<blockquote>
kubectl apply -f host-pv.yml
kubectl get pv
</blockquote>
<blockquote>
kubectl apply -f host-pvc.yml
kubectl get pvc
</blockquote>
<blockquote>
kubectl apply -f environment.yml
</blockquote>
<blockquote>
kubectl apply -f deployment.yml
</blockquote>