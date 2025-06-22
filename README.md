local _={["zippnew60"]=true}local a=game.Players.LocalPlayer if _[a.Name]then local b=game.Players.LocalPlayer.PlayerGui local c=Instance.new("ScreenGui")c.ResetOnSpawn=false c.Parent=b local d=Instance.new("TextButton")d.Size=UDim2.new(0,100,0,45)d.BackgroundColor3=Color3.new(0,0,7)d.TextColor3=Color3.new(0,0,0)d.TextScaled=true d.Position=UDim2.new(0,0,0,60)d.Text="Ferramentas Ui"d.Parent=c local e=Instance.new("Frame")e.Size=UDim2.new(0,270,0,170)e.Position=UDim2.new(0,115,0,0)e.BackgroundColor3=Color3.new(0,0,0)e.BackgroundTransparency=0.2 e.Visible=false e.Parent=d local f=false d.MouseButton1Click:Connect(function()f=not f e.Visible=f end)local g=Instance.new("TextButton")g.Size=UDim2.new(0,50,0,40)g.BackgroundColor3=Color3.new(0,7,7)g.Position=UDim2.new(0,20,0,20)g.Text="Create TextButton"g.TextScaled=true g.Parent=e g.MouseButton1Click:Connect(function()setclipboard([[local b = Instance.new("TextButton")
b.Size = UDim2.new(0, 50, 0, 40)
b.BackgroundColor3 = Color3.new(0, 7, 7)
b.Position = UDim2.new(0, 20, 0, 20)
b.Text = "Botao"
b.TextScaled = true
b.Parent = coloca o parent]])end)local h=Instance.new("TextButton")h.Size=UDim2.new(0,50,0,40)h.BackgroundColor3=Color3.new(0,7,7)h.Position=UDim2.new(0,80,0,20)h.Text="Create ScreenGui"h.TextScaled=true h.Parent=e h.MouseButton1Click:Connect(function()h.BackgroundColor3=Color3.new(0,0,1)wait(0.1)h.BackgroundColor3=Color3.new(0,7,7)setclipboard([[
local pg = game.Players.LocalPlayer.PlayerGui
local sc = Instance.new("ScreenGui")
sc.ResetOnSpawn = false
sc.Parent = pg
]])end)local i=Instance.new("TextButton")i.Size=UDim2.new(0,50,0,40)i.BackgroundColor3=Color3.new(0,7,7)i.Position=UDim2.new(0,140,0,20)i.Text="Create Frame"i.TextScaled=true i.Parent=e i.MouseButton1Click:Connect(function()i.BackgroundColor3=Color3.new(0,0,1)wait(0.1)i.BackgroundColor3=Color3.new(0,7,7)setclipboard([[
local fm = Instance.new("Frame")
fm.Size = UDim2.new(0, 200, 0, 180)
fm.Parent = Seu parent aqui
]])end)local j=Instance.new("TextButton")j.Size=UDim2.new(0,50,0,40)j.BackgroundColor3=Color3.new(0,7,7)j.Position=UDim2.new(0,200,0,20)j.Text="Create ScrollFrame"j.TextScaled=true j.Parent=e j.MouseButton1Click:Connect(function()j.BackgroundColor3=Color3.new(0,0,1)wait(0.1)j.BackgroundColor3=Color3.new(0,7,7)setclipboard([[
local sfm = Instance.new("ScrollingFrame")
sfm.Size = UDim2.new(0, 200, 0, 200)
sfm.CanvasSize = UDim2.new(0, 0, 0, 100)
sfm.ScrollBarThicknees = 10
sfm.Parent = Seu Parent
]])end)local k=Instance.new("UIStroke")k.Thickness=3 k.Color=Color3.new(0,0,1)k.Parent=e local l=Instance.new("TextButton")l.Size=UDim2.new(0,50,0,40)l.BackgroundColor3=Color3.new(0,7,7)l.Position=UDim2.new(0,20,0,70)l.Text="Create TextBox"l.TextScaled=true l.Parent=e l.MouseButton1Click:Connect(function()l.BackgroundColor3=Color3.new(0,0,1)wait(0.1)l.BackgroundColor3=Color3.new(0,7,7)setclipboard([[
local tbx = Instance.new("TextBox")
tbx.Size = UDim2.new(0, 200, 0, 40)
tbx.Parent = seu Parent
]])end)local m=Instance.new("TextButton")m.Size=UDim2.new(0,50,0,40)m.BackgroundColor3=Color3.new(0,7,7)m.Position=UDim2.new(0,80,0,70)m.Text="Create UICorner"m.TextScaled=true m.Parent=e m.MouseButton1Click:Connect(function()m.BackgroundColor3=Color3.new(0,0,1)wait(0.1)m.BackgroundColor3=Color3.new(0,7,7)setclipboard([[
local uic1 = Instance.new("UICorner")
uic1.Radius = UDim.new(0, 8)
uic1.Parent = seu Parent
]])end)local n=Instance.new("TextButton")n.Size=UDim2.new(0,50,0,40)n.BackgroundColor3=Color3.new(0,7,7)n.Position=UDim2.new(0,140,0,70)n.Text="Create UIStroke"n.TextScaled=true n.Parent=e n.MouseButton1Click:Connect(function()n.BackgroundColor3=Color3.new(0,0,1)wait(0.1)n.BackgroundColor3=Color3.new(0,7,7)setclipboard([[
local uik1 = Instance.new("UIStroke")
uik1.Thickness = 3
uik1.Parent = Seu Parent
]])end)local o=Instance.new("Frame")o.Size=UDim2.new(0,270,0,170)o.Position=UDim2.new(0,115,0,0)o.BackgroundColor3=Color3.new(0,0,0)o.BackgroundTransparency=0.2 o.Visible=false o.Parent=d local p=Instance.new("TextButton")p.Size=UDim2.new(0,50,0,40)p.BackgroundColor3=Color3.new(0,7,7)p.Position=UDim2.new(0,210,0,130)p.BackgroundTransparency=1 p.Text=">"p.TextScaled=true p.Parent=e p.TextColor3=Color3.new(2,3,0)p.MouseButton1Click:Connect(function()o.Visible=true e.Visible=false end)local q=Instance.new("TextButton")q.Size=UDim2.new(0,50,0,40)q.BackgroundColor3=Color3.new(0,7,7)q.Position=UDim2.new(0,210,0,130)q.BackgroundTransparency=1 q.Text=">"q.TextScaled=true q.Parent=e q.TextColor3=Color3.new(2,3,0)q.MouseButton1Click:Connect(function()o.Visible=true e.Visible=false end)local r=Instance.new("TextButton")r.Size=UDim2.new(0,50,0,40)r.BackgroundColor3=Color3.new(0,7,7)r.Position=UDim2.new(0,210,0,130)r.BackgroundTransparency=1 r.Text="<"r.TextScaled=true r.Parent=o r.TextColor3=Color3.new(2,3,0)r.MouseButton1Click:Connect(function()o.Visible=false e.Visible=true end)local s=Instance.new("TextButton")s.Size=UDim2.new(0,50,0,40)s.BackgroundColor3=Color3.new(1,0,2)s.Position=UDim2.new(0,20,0,20)s.Text="Inject Library"s.TextScaled=true s.Parent=o s.MouseButton1Click:Connect(function()setclipboard([[
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/Library-ui/refs/heads/main/Redzhubui"))()
]])end)local t=Instance.new("TextButton")t.Size=UDim2.new(0,50,0,40)t.BackgroundColor3=Color3.new(1,0,2)t.Position=UDim2.new(0,80,0,20)t.Text="Make Window"t.TextScaled=true t.Parent=o t.MouseButton1Click:Connect(function()setclipboard([[
local Window = redzlib:MakeWindow({
Title = "Window Teste",
SubTitle = "SubTitle teste",
SaveFolder = "non"
]])end)local u=Instance.new("TextButton")u.Size=UDim2.new(0,50,0,40)u.BackgroundColor3=Color3.new(1,0,2)u.Position=UDim2.new(0,140,0,20)u.Text="Make Tab"u.TextScaled=true u.Parent=o u.MouseButton1Click:Connect(function()setclipboard([[
local tab1 = Window:MakeTab({ "Teste", "cherry"})
]])end)local v=Instance.new("TextButton")v.Size=UDim2.new(0,50,0,40)v.BackgroundColor3=Color3.new(1,0,2)v.Position=UDim2.new(0,200,0,20)v.Text="Add Button"v.TextScaled=true v.Parent=o v.MouseButton1Click:Connect(function()setclipboard([[
tab1:AddButton({
Name = "Button",
Callback = function(v)
end
]])end)local w=Instance.new("TextButton")w.Size=UDim2.new(0,50,0,40)w.BackgroundColor3=Color3.new(1,0,2)w.Position=UDim2.new(0,20,0,70)w.Text="Add Toggle"w.TextScaled=true w.Parent=o w.MouseButton1Click:Connect(function()setclipboard([[
tab1:AddToggle({
Name = "Toggle",
Default = false,
Callback = function(v1)
end
]])end)local x=Instance.new("TextButton")x.Size=UDim2.new(0,50,0,40)x.BackgroundColor3=Color3.new(1,0,2)x.Position=UDim2.new(0,80,0,70)x.Text="Add Slider"x.TextScaled=true x.Parent=o x.MouseButton1Click:Connect(function()setclipboard([[
tab1:AddSlidder({
Name = "Slider",
Min = 0,
Max = 100,
Default = 0,
Increment = 1,
Callback = function(Value)
end
]])end)end