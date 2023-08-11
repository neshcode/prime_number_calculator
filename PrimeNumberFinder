import json

def lambda_handler(event,context):
    non_prime=[]
    prime=[]
    data=event["data"]
    for num in data:
        for i in range(2,num):
            if num%i==0:
                non_prime.append(num)
                break
            if i==(num-1):
                prime.append(num)
            list={"Non-Prime":non_prime,
              "Prime":prime}
        
    return json.dumps(list)
