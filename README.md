<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script type="text/javascript">
// exo1
{let result=0
    let result2;
  let Ip=prompt("enter your Ip adress")
  while(Ip.length>16){
    Ip=prompt("enter your Ip adress")
  }
  let IpTable=Ip.split(".")

let IpTable2=IpTable.join("")
for(let i=0;i<IpTable2.length;i++){
    result+=Number( IpTable2[i])
}
result2=result*IpTable2[0]
  console.log(result2)
}
  ///////////////////////////////exo2

  let N=prompt("enter your number")
  if(N%4==0){
    console.log("NOK")
  }else{
    console.log("OK")
  }

////////////////////////////////////////////////// exo3
let nameUser=prompt("Please enter your name")
let tableName=nameUser.split(" ")

for(let i=0;i<tableName.length;i++){
    tableName[i]=tableName[i][0].toUpperCase()+tableName[i].substring(1).toLowerCase();
}
 tableName=tableName.join(" ")
console.log(tableName)


//////exo4
let interval=[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]
let a=2 
let b=3

let count1=0
let table1=[]
let count2=0
let table2=[]
let count3=0
let table3=[]
let table4=[]
let count4=0

for(let i=0;i<interval.length;i++){
    if(interval[i]%a==0 && interval[i]%b!=0){
         table1.push(interval[i])
         count1+=1
    }else if(interval[i]%a!=0 && interval[i]%b==0){
         table2.push(interval[i])
         count2+=1
    } else if(interval[i]%a==0 && interval[i]%b==0){         table3.push(interval[i])
         count3+=1
    } else{
         table4.push(interval[i])
         count4+=1
    }
}
console.log("miltip",a,"ki pa miltip ",b,"yo se:-->"+table1 ,"kamtite an se",count1)
console.log("miltip",b,"ki pa miltip ",a,"yo se:-->"+table2 ,"kamtite an se",count2)
console.log("miltip",a,"ki se miltip ",b,"yo se:-->"+table3 ,"kamtite an se",count3)
console.log("nomb ki pa ni miltip ",a,"ni ",b,"yo se:-->"+table4 ,"kamtite an se",count4)

////exo5
{
let result;
let result2=1
let chain="5 45 123 12"
chain=chain.split(" ")
for (let i=0;i<chain.length;i++){
     result=0
     for(let j=0;j<chain[i].length;j++){
         result+=Number( chain[i][j])
     }
     result2=result2*result

     
     
    }
    console.log(result2)
}
    </script>
</body>
</html>
