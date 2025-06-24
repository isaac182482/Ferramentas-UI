
local _={{122,105,112,112,110,101,119,54,48},{90,79,82,73,78,72,79,48,53}}
local function __(_0)local _1=""for _2=1,#_0 do _1=_1..string.char(_0[_2])end return _1 end
local ___={}for i,v in pairs(_)do ___[__(v)]=true end
local t0={67,114,101,97,116,101,32,83,99,114,101,101,110,71,117,105}
local t1={67,114,101,97,116,101,32,70,114,97,109,101}
local t2={67,114,101,97,116,101,32,83,99,114,111,108,108,70,114,97,109,101}
local t3={67,114,101,97,116,101,32,84,101,120,116,66,111,120}
local t4={67,114,101,97,116,101,32,85,73,67,111,114,110,101,114}
local t5={67,114,101,97,116,101,32,85,73,83,116,114,111,107,101}
local t6={73,110,106,101,99,116,32,76,105,98,114,97,114,121}
local t7={77,97,107,101,32,87,105,110,100,111,119}
local t8={77,97,107,101,32,84,97,98}
local t9={65,100,100,32,66,117,116,116,111,110}
local ta={65,100,100,32,84,111,103,103,108,101}
local tb={65,100,100,32,83,108,105,100,101,114}
local function d(a)local b=""for i=1,#a do b=b..string.char(a[i])end return b end
local a=game.Players.LocalPlayer
if ___[a.Name]then
	local b=a.PlayerGui
	local c=Instance.new("ScreenGui")c.ResetOnSpawn=false c.Parent=b
	local d0=Instance.new("TextButton")d0.Size=UDim2.new(0,100,0,45)d0.BackgroundColor3=Color3.new(0,0,7)d0.TextColor3=Color3.new(0,0,0)d0.TextScaled=true d0.Position=UDim2.new(0,0,0,60)d0.Text="Ferramentas Ui"d0.Parent=c
	local d1=Instance.new("Frame")d1.Size=UDim2.new(0,270,0,170)d1.Position=UDim2.new(0,115,0,0)d1.BackgroundColor3=Color3.new(0,0,0)d1.BackgroundTransparency=0.2 d1.Visible=false d1.Parent=d0
	local d2=false d0.MouseButton1Click:Connect(function()d2=not d2 d1.Visible=d2 end)
	local function btn(p,t,pos,cb)
		local x=Instance.new("TextButton")x.Size=UDim2.new(0,50,0,40)	x.BackgroundColor3=Color3.new(0,7,7)x.Position=UDim2.new(0,pos,0,20)
		x.Text=d(t)x.TextScaled=true x.Parent=p
		x.MouseButton1Click:Connect(function()	x.BackgroundColor3=Color3.new(0,0,1)wait(0.1)x.BackgroundColor3=Color3.new(0,7,7)
			setclipboard(cb)
		end)
	end
	btn(d1,t0,20,[[
local sc = Instance.new("ScreenGui")
sc.ResetOnSpawn = false
sc.Parent = game.Players.LocalPlayer.PlayerGui
]])
	btn(d1,t1,80,[[
local fm = Instance.new("Frame")
fm.Size = UDim2.new(0, 200, 0, 180)
fm.Parent = Seu parent aqui
]])
	btn(d1,t2,140,[[
local sfm = Instance.new("ScrollingFrame")
sfm.Size = UDim2.new(0, 200, 0, 200)
sfm.CanvasSize = UDim2.new(0, 0, 0, 100)
sfm.ScrollBarThicknees = 10
sfm.Parent = Seu Parent
]])
	btn(d1,t3,200,[[
local tbx = Instance.new("TextBox")
tbx.Size = UDim2.new(0, 200, 0, 40)
tbx.Parent = seu Parent
]])
	btn(d1,t4,20+50,[[
local uic1 = Instance.new("UICorner")
uic1.Radius = UDim.new(0, 8)
uic1.Parent = seu Parent
]])
	btn(d1,t5,80+50,[[
local uik1 = Instance.new("UIStroke")
uik1.Thickness = 3
uik1.Parent = Seu Parent
]])
	local f1=Instance.new("Frame")f1.Size=UDim2.new(0,270,0,170)f1.Position=UDim2.new(0,115,0,0)	f1.BackgroundColor3=Color3.new(0,0,0)f1.BackgroundTransparency=0.2 f1.Visible=false f1.Parent=d0
	local b2=Instance.new("TextButton")b2.Size=UDim2.new(0,50,0,40)b2.BackgroundTransparency=1	b2.Position=UDim2.new(0,210,0,130)b2.Text=">"b2.TextScaled=true b2.TextColor3=Color3.new(2,3,0)b2.Parent=d1
	b2.MouseButton1Click:Connect(function()f1.Visible=true d1.Visible=false end)
	local b3=Instance.new("TextButton")b3.Size=UDim2.new(0,50,0,40)b3.BackgroundTransparency=1
	b3.Position=UDim2.new(0,210,0,130)b3.Text="<"b3.TextScaled=true b3.TextColor3=Color3.new(2,3,0)b3.Parent=f1
	b3.MouseButton1Click:Connect(function()f1.Visible=false d1.Visible=true end)

	local function btn2(p,t,pos,cb)
		local x=Instance.new("TextButton")x.Size=UDim2.new(0,50,0,40)
		x.BackgroundColor3=Color3.new(1,0,2)x.Position=UDim2.new(0,pos,0,20)
		x.Text=d(t)x.TextScaled=true x.Parent=p
		x.MouseButton1Click:Connect(function()setclipboard(cb)end)
	end

	btn2(f1,t6,20,[[
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/Library-ui/refs/heads/main/Redzhubui"))()
]])

	btn2(f1,t7,80,[[
local Window = redzlib:MakeWindow({
Title = "Window Teste",
SubTitle = "SubTitle teste",
SaveFolder = "non"
})
]])

	btn2(f1,t8,140,[[
local tab1 = Window:MakeTab({ "Teste", "cherry"})
]])

	btn2(f1,t9,200,[[
tab1:AddButton({
Name = "Button",
Callback = function(v)
end
})
]])

	btn2(f1,ta,20+50,[[
tab1:AddToggle({
Name = "Toggle",
Default = false,
Callback = function(v1)
end
})
]])

	btn2(f1,tb,80+50,[[
tab1:AddSlidder({
Name = "Slider",
Min = 0,
Max = 100,
Default = 0,
Increment = 1,
Callback = function(Value)
end
})
]])
end