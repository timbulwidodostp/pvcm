# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Variable Coefficients Models for Panel Data Use pvcm (plm) With (In) R Software
install.packages("plm")
library("plm")
# Estimation Variable Coefficients Models for Panel Data Use pvcm (plm) With (In) R Software
pvcm = read.csv("https://raw.githubusercontent.com/timbulwidodostp/pvcm/main/pvcm/pvcm.csv", sep = ";")
pvcm_data <- as.data.frame(pvcm)
pvcm <- pvcm(Dependen ~ Indenpenden_1 + Indenpenden_2, data = pvcm_data, model = "within")
pvcm_ <- pvcm(Dependen ~ Indenpenden_1 + Indenpenden_2, data = pvcm_data, model = "random")
summary(pvcm(Dependen ~ Indenpenden_1 + Indenpenden_2, data = pvcm_data, model = "random"))
# Variable Coefficients Models for Panel Data Use pvcm (plm) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
