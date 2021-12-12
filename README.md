<!DOCTYPE html>
<html>
<head>
   <title></title>
<style>
  *
{
  margin:0;
  padding:0;
  box-sizing:border-box;
}
  body
{
  display:flex;
  align-items:center;
  justify-content:center;
  height:100vh;
  background:#0e1538;
}
  .box
{
  position:relative;
  height:400px;
  width:300px;
  display:flex;
  align-items:center;
  justify-content:center;
  background:rgba(0,0,0,0.5);
  overflow: hidden;
  border-radius:20px;
}
  .box::after
{
  content:"";
  position: absolute;
  inset:4px;
  background:#0e1538;
  border-radius:20px;
}
  .box::before
{
  content:"";
  position: absolute;
  width:150px;
  height:140%;
  background:linear-gradient(#00ccff,#d400d4);
  animation: animate 4s linear infinite;
}
  @keyframes animate
{
  0%
  {
    transform:rotate(0deg);
  }
  100%
  {
    transform:rotate(360deg);
  }
}
  .box h2
{
  position:relative;
  color:#fff;
  font-size:8em;
  z-index:10;
}
</style>
</head>
<body>
  <div class="box">
    <h2>02</h2>
  </div>
</body>
</html>
