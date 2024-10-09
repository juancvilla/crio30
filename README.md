# crio30

Ref.- https://www.linuxtechi.com/how-to-install-kubernetes-cluster-rhel/

git clone https://github.com/juancvilla/crio30

subscription-manager register --username jvillarroelquintec --auto-attach

cd $HOME/crio30

sudoers + wheel

sh script.sh 

On master:

sh master.sh

On Worker:

sudo kubeadm join 192.168.100.247:6443 --token vd23kx.s30ddxxl3dcliqg0 --discovery-token-ca-cert-hash sha256:dde449b68b921faf407b83cfb860e31b6bf0b5199ff881386773fa36b2255ba9 
