local a={}a[string.char(122,105,112,112,110,101,119,54,48)]=true
local b=game:GetService(string.char(80,108,97,121,101,114,115)).LocalPlayer
local function c()
local d=b:WaitForChild(string.char(80,108,97,121,101,114,71,117,105))
local e=Instance.new(string.char(83,99,114,101,101,110,71,117,105))
e.ResetOnSpawn=false e.Parent=d
local f=Instance.new(string.char(84,101,120,116,66,117,116,116,111,110))
f.Size=UDim2.new(0,100,0,45)f.BackgroundColor3=Color3.new(0,0,7)
f.TextColor3=Color3.new(0,0,0)f.TextScaled=true
f.Position=UDim2.new(0,0,0,60)
f.Text=string.char(70,101,114,114,97,109,101,110,116,97,115,32,85,105)
f.Parent=e
local g=Instance.new(string.char(70,114,97,109,101))
g.Size=UDim2.new(0,270,0,170)
g.Position=UDim2.new(0,115,0,0)
g.BackgroundColor3=Color3.new(0,0,0)
g.BackgroundTransparency=0.2
g.Visible=false g.Parent=f
local h=false
f.MouseButton1Click:Connect(function()
h=not h g.Visible=h end)

local function i(j,k,l,m,n)local o=Instance.new("TextButton")
o.Size=UDim2.new(0,50,0,40)
o.BackgroundColor3=Color3.new(0,7,7)
o.Position=UDim2.new(0,k,0,l)
o.Text=m o.TextScaled=true o.Parent=g
o.MouseButton1Click:Connect(function()
o.BackgroundColor3=Color3.new(0,0,1)wait(.1)
o.BackgroundColor3=Color3.new(0,7,7)
setclipboard(n)end)end

i(1,20,20,"B"..string.char(111,116,97,111),[[local b=Instance.new("TextButton")b.Size=UDim2.new(0,50,0,40)b.BackgroundColor3=Color3.new(0,7,7)b.Position=UDim2.new(0,20,0,20)b.Text="Botao"b.TextScaled=true b.Parent=coloca o parent]])
i(2,80,20,"S"..string.char(99),[[local pg=game.Players.LocalPlayer.PlayerGui local sc=Instance.new("ScreenGui")sc.ResetOnSpawn=false sc.Parent=pg]])
i(3,140,20,"F"..string.char(114,97,109,101),[[local fm=Instance.new("Frame")fm.Size=UDim2.new(0,200,0,180)fm.Parent=Seu parent aqui]])
i(4,200,20,"S"..string.char(99,114,111,108),[[local sfm=Instance.new("ScrollingFrame")sfm.Size=UDim2.new(0,200,0,200)sfm.CanvasSize=UDim2.new(0,0,0,100)sfm.ScrollBarThicknees=10 sfm.Parent=Seu Parent]])
local p=Instance.new("UIStroke")
p.Thickness=3 p.Color=Color3.new(0,0,1)
p.Parent=g
i(5,20,70,"T"..string.char(98),[[local tbx=Instance.new("TextBox")tbx.Size=UDim2.new(0,200,0,40)tbx.Parent=seu Parent]])
i(6,80,70,"U"..string.char(105,67),[[local uic1=Instance.new("UICorner")uic1.Radius=UDim.new(0,8)uic1.Parent=seu Parent]])
i(7,140,70,"U"..string.char(105,83),[[local uik1=Instance.new("UIStroke")uik1.Thickness=3 uik1.Parent=Seu Parent]])
end

if a[b.Name]then(c)()end