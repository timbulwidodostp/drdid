# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Doubly Robust Difference in Difference (DID) with Multiple periods estimator Use drdid With (In) R Software
install.packages("DRDID")
library("DRDID")
drdid = read.csv("https://raw.githubusercontent.com/timbulwidodostp/drdid/main/drdid/drdid.csv",sep = ";")
# Estimates Two Stage Difference in Differences (DID) Use did2s With (In) R Software
drdid<-drdid(yname="re",tname="year",idname="id",dname="experimental",xformla=~age+educ+black+married+nodegree+hisp+re74,data=drdid,panel=TRUE)
summary(drdid)

# Doubly Robust Difference in Difference (DID) with Multiple periods estimator Use drdid With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
