        local pg = game.Players.LocalPlayer.PlayerGui
local sc = Instance.new("ScreenGui")
sc.ResetOnSpawn = false
sc.Parent = pg
--Barra de MenuUi
local br = Instance.new("TextButton")
br.Size = UDim2.new(0, 100, 0, 45)
br.BackgroundColor3 = Color3.new(0, 0, 7)
br.TextColor3 = Color3.new(0, 0, 0)
br.TextScaled = true
br.Position = UDim2.new(0, 0, 0, 60)
br.Text = "Ferramentas Ui"
br.Parent = sc

--Frame Fundo
local fd = Instance.new("Frame")
fd.Size = UDim2.new(0, 270, 0, 170)
fd.Position = UDim2.new(0, 115, 0, 0)
fd.BackgroundColor3 = Color3.new(0, 0, 0)
fd.BackgroundTransparency = 0.2
fd.Visible = false
fd.Parent = br

--Mostrar fd
v = false
br.MouseButton1Click:Connect(function()
v = not v
fd.Visible = v
end)

--botao 1, criar botoes
local b1 = Instance.new("TextButton")
b1.Size = UDim2.new(0, 50, 0, 40)
b1.BackgroundColor3 = Color3.new(0, 7, 7)
b1.Position = UDim2.new(0, 20, 0, 20)
b1.Text = "Create TextButton"
b1.TextScaled = true
b1.Parent = fd

b1.MouseButton1Click:Connect(function()
setclipboard([[local b = Instance.new("TextButton")
b.Size = UDim2.new(0, 50, 0, 40)
b.BackgroundColor3 = Color3.new(0, 7, 7)
b.Position = UDim2.new(0, 20, 0, 20)
b.Text = "Botao"
b.TextScaled = true
b.Parent = coloca o parent]])
end)

--botao 2, criar Screen
local b2 = Instance.new("TextButton")
b2.Size = UDim2.new(0, 50, 0, 40)
b2.BackgroundColor3 = Color3.new(0, 7, 7)
b2.Position = UDim2.new(0, 80, 0, 20)
b2.Text = "Create ScreenGui"
b2.TextScaled = true
b2.Parent = fd

b2.MouseButton1Click:Connect(function()
b2.BackgroundColor3 = Color3.new(0, 0, 1)
wait(0.1)
b2.BackgroundColor3 = Color3.new(0, 7, 7)
setclipboard([[
     local pg = game.Players.LocalPlayer.PlayerGui
local sc = Instance.new("ScreenGui")
sc.ResetOnSpawn = false
sc.Parent = pg
]])
end)

--botao 3, criar Frame
local b3 = Instance.new("TextButton")
b3.Size = UDim2.new(0, 50, 0, 40)
b3.BackgroundColor3 = Color3.new(0, 7, 7)
b3.Position = UDim2.new(0, 140, 0, 20)
b3.Text = "Create Frame"
b3.TextScaled = true
b3.Parent = fd

b3.MouseButton1Click:Connect(function()
b3.BackgroundColor3 = Color3.new(0, 0, 1)
wait(0.1)
b3.BackgroundColor3 = Color3.new(0, 7, 7)
setclipboard([[
local fm = Instance.new("Frame")
fm.Size = UDim2.new(0, 200, 0, 180)
fm.Parent = Seu parent aqui
]])
end)

--botao 4, criar ScrollingFrame
local b4 = Instance.new("TextButton")
b4.Size = UDim2.new(0, 50, 0, 40)
b4.BackgroundColor3 = Color3.new(0, 7, 7)
b4.Position = UDim2.new(0, 200, 0, 20)
b4.Text = "Create ScrollFrame"
b4.TextScaled = true
b4.Parent = fd

b4.MouseButton1Click:Connect(function()
b4.BackgroundColor3 = Color3.new(0, 0, 1)
wait(0.1)
b4.BackgroundColor3 = Color3.new(0, 7, 7)
setclipboard([[
local sfm = Instance.new("ScrollingFrame")
sfm.Size = UDim2.new(0, 200, 0, 200)
sfm.CanvasSize = UDim2.new(0, 0, 0, 100)
sfm.ScrollBarThicknees = 10
sfm.Parent = Seu Parent
]])
end)

local uis1 = Instance.new("UIStroke")
uis1.Thickness = 3
uis1.Color = Color3.new(0, 0, 1)
uis1.Parent = fd
--botao 5, criar TextBox
local b5 = Instance.new("TextButton")
b5.Size = UDim2.new(0, 50, 0, 40)
b5.BackgroundColor3 = Color3.new(0, 7, 7)
b5.Position = UDim2.new(0, 20, 0, 70)
b5.Text = "Create TextBox"
b5.TextScaled = true
b5.Parent = fd

b5.MouseButton1Click:Connect(function()
b5.BackgroundColor3 = Color3.new(0, 0, 1)
wait(0.1)
b5.BackgroundColor3 = Color3.new(0, 7, 7)
setclipboard([[
local tbx = Instance.new("TextBox")
tbx.Size = UDim2.new(0, 200, 0, 40)
tbx.Parent = seu Parent
]])
end)

--botao 6, criar UiCorner
local b6 = Instance.new("TextButton")
b6.Size = UDim2.new(0, 50, 0, 40)
b6.BackgroundColor3 = Color3.new(0, 7, 7)
b6.Position = UDim2.new(0, 80, 0, 70)
b6.Text = "Create UICorner"
b6.TextScaled = true
b6.Parent = fd

b6.MouseButton1Click:Connect(function()
b6.BackgroundColor3 = Color3.new(0, 0, 1)
wait(0.1)
b6.BackgroundColor3 = Color3.new(0, 7, 7)
setclipboard([[
local uic1 = Instance.new("UICorner")
uic1.Radius = UDim.new(0, 8)
uic1.Parent = seu Parent
]])
end)

 
