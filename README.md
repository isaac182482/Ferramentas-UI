
local _ = {["zippnew60"] = true}
local a = game.Players.LocalPlayer

if _[a.Name] then
	local b = a.PlayerGui
	local c = Instance.new("ScreenGui")
	c.ResetOnSpawn = false
	c.Parent = b
	local d = Instance.new("TextButton")
	d.Size = UDim2.new(0, 100, 0, 45)
	d.BackgroundColor3 = Color3.new(0, 0, 7)
	d.TextColor3 = Color3.new(0, 0, 0)
	d.TextScaled = true
	d.Position = UDim2.new(0, 0, 0, 60)
	d.Text = "Ferramentas Ui"
	d.Parent = c
	local e = Instance.new("Frame")
	e.Size = UDim2.new(0, 270, 0, 170)
	e.Position = UDim2.new(0, 115, 0, 0)
	e.BackgroundColor3 = Color3.new(0, 0, 0)
	e.BackgroundTransparency = 0.2
	e.Visible = false
	e.Parent = d
	local f = false
	d.MouseButton1Click:Connect(function()
		f = not f
		e.Visible = f
	end)
	local function createButton(name, posX, posY, clipboardContent, parent)
		local btn = Instance.new("TextButton")
		btn.Size = UDim2.new(0, 50, 0, 40)
		btn.Position = UDim2.new(0, posX, 0, posY)
		btn.BackgroundColor3 = Color3.new(0, 7, 7)
		btn.Text = name
		btn.TextScaled = true
		btn.Parent = parent
		btn.MouseButton1Click:Connect(function()
			btn.BackgroundColor3 = Color3.new(0, 0, 1)
			wait(0.1)
			btn.BackgroundColor3 = Color3.new(0, 7, 7)
			setclipboard(clipboardContent)
		end)
	end
	createButton("Create TextButton", 20, 20, [[
local b = Instance.new("TextButton")
b.Size = UDim2.new(0, 50, 0, 40)
b.BackgroundColor3 = Color3.new(0, 7, 7)
b.Position = UDim2.new(0, 20, 0, 20)
b.Text = "Botao"
b.TextScaled = true
b.Parent = coloca o parent
]], e)
	createButton("Create ScreenGui", 80, 20, [[
local pg = game.Players.LocalPlayer.PlayerGui
local sc = Instance.new("ScreenGui")
sc.ResetOnSpawn = false
sc.Parent = pg
]], e)
	createButton("Create Frame", 140, 20, [[
local fm = Instance.new("Frame")
fm.Size = UDim2.new(0, 200, 0, 180)
fm.Parent = Seu parent aqui
]], e)
	createButton("Create ScrollFrame", 200, 20, [[
local sfm = Instance.new("ScrollingFrame")
sfm.Size = UDim2.new(0, 200, 0, 200)
sfm.CanvasSize = UDim2.new(0, 0, 0, 100)
sfm.ScrollBarThickness = 10
sfm.Parent = Seu Parent
]], e)
	createButton("Create TextBox", 20, 70, [[
local tbx = Instance.new("TextBox")
tbx.Size = UDim2.new(0, 200, 0, 40)
tbx.Parent = seu Parent
]], e)
	createButton("Create UICorner", 80, 70, [[
local uic1 = Instance.new("UICorner")
uic1.Radius = UDim.new(0, 8)
uic1.Parent = seu Parent
]], e)
	createButton("Create UIStroke", 140, 70, [[
local uik1 = Instance.new("UIStroke")
uik1.Thickness = 3
uik1.Parent = Seu Parent
]], e)
	local k = Instance.new("UIStroke")
	k.Thickness = 3
	k.Color = Color3.new(0, 0, 1)
	k.Parent = e
	local o = Instance.new("Frame")
	o.Size = UDim2.new(0, 270, 0, 170)
	o.Position = UDim2.new(0, 115, 0, 0)
	o.BackgroundColor3 = Color3.new(0, 0, 0)
	o.BackgroundTransparency = 0.2
	o.Visible = false
	o.Parent = d
	local function createNavButton(parent, targetToShow, targetToHide, text, x)
		local btn = Instance.new("TextButton")
		btn.Size = UDim2.new(0, 50, 0, 40)
		btn.Position = UDim2.new(0, x, 0, 130)
		btn.BackgroundTransparency = 1
		btn.BackgroundColor3 = Color3.new(0, 7, 7)
		btn.Text = text
		btn.TextScaled = true
		btn.TextColor3 = Color3.new(2, 3, 0)
		btn.Parent = parent
		btn.MouseButton1Click:Connect(function()
			targetToShow.Visible = true
			targetToHide.Visible = false
		end)
	end
	createNavButton(e, o, e, ">", 210)
	createNavButton(o, e, o, "<", 210)
	local function createLibraryButton(name, posX, posY, clipboardContent)
		local btn = Instance.new("TextButton")
		btn.Size = UDim2.new(0, 50, 0, 40)
		btn.Position = UDim2.new(0, posX, 0, posY)
		btn.BackgroundColor3 = Color3.new(1, 0, 2)
		btn.Text = name
		btn.TextScaled = true
		btn.Parent = o
		btn.MouseButton1Click:Connect(function()
			setclipboard(clipboardContent)
		end)
	end
	createLibraryButton("Inject Library", 20, 20, [[
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/Library-ui/refs/heads/main/Redzhubui"))()
]])
	createLibraryButton("Make Window", 80, 20, [[
local Window = redzlib:MakeWindow({
	Title = "Window Teste",
	SubTitle = "SubTitle teste",
	SaveFolder = "non"
})
]])
	createLibraryButton("Make Tab", 140, 20, [[
local tab1 = Window:MakeTab({ "Teste", "cherry" })
]])
createLibraryButton("Add Button", 200, 20, [[
tab1:AddButton({
	Name = "Button",
	Callback = function(v)
	end
})
]])
createLibraryButton("Add Toggle", 20, 70, [[
tab1:AddToggle({
	Name = "Toggle",
	Default = false,
	Callback = function(v1)
	end
})
]])
createLibraryButton("Add Slider", 80, 70, [[
tab1:AddSlider({
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