# Fitness_TrackerRun

 133  git clone https://github.com/rahuldutta0487/Fitness_Tracker.git
  134  ls
  135  cd Fitness_Tracker
  136  ls
  137  nano Dockerfile
  138  docker build -t rahuldutta0487/fitness-tracker:v1 .
  139  docker run -d --name fitness-app -p 5000:5000 rahuldutta0487/fitness-trac                                                       ker:v1
  140  curl http://localhost:5000
  141  docker ps
  142  docker rm -f hospital-app fitness-app
  143  docker run -d --name fitness-app -p 5001:5000 rahuldutta0487/fitness-trac                                                       ker:v1
  144  curl http://localhost:5001
  145  http://YOUR_EC2_PUBLIC_IP:5001
  146  curl ifconfig.me
  147  aws eks update-kubeconfig --region ap-south-1 --name fitness-prod-cluster
  148  kubectl get nodes
  149  kubectl get pods -A
  150  kubectl get svc
  151  kubectl delete deployment hospital-app
  152  kubectl delete svc hospital-service
  153  kubectl delete statefulset mongodb
  154  kubectl create deployment fitness-app   --image=rahuldutta0487/fitness-tr                                                       acker:v1   --port=5000
  155  kubectl expose deployment fitness-app   --type=LoadBalancer   --name=fitn                                                       ess-service   --port=80   --target-port=5000
  156  kubectl get pods
  157  kubectl get svc
  158  kubectl describe pod fitness-app-8c8bcc844-9ctfv
  159  docker images
  160  docker login
  161  docker push rahuldutta0487/fitness-tracker:v1
  162  docker pull rahuldutta0487/fitness-tracker:v1
  163  kubectl rollout restart deployment fitness-app
  164  kubectl get pods -w
  165  history
root@ip-172-31-0-247:/home/ubuntu/Fitness_Tracker#
