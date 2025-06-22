local _wl = {["zippnew60"] = true}
local _plr = game.Players.LocalPlayer

local function _Fx()
    local _pg = _plr:WaitForChild("PlayerGui")
    local _sc = Instance.new("ScreenGui")
    _sc.ResetOnSpawn = false
    _sc.Parent = _pg

    local _b = Instance.new("TextButton")
    _b.Size = UDim2.new(0, 100, 0, 45)
    _b.BackgroundColor3 = Color3.new(0, 0, 7)
    _b.TextColor3 = Color3.new(0, 0, 0)
    _b.TextScaled = true
    _b.Position = UDim2.new(0, 0, 0, 60)
    _b.Text = "Ferramentas Ui"
    _b.Parent = _sc

    local _f = Instance.new("Frame")
    _f.Size = UDim2.new(0, 270, 0, 170)
    _f.Position = UDim2.new(0, 115, 0, 0)
    _f.BackgroundColor3 = Color3.new(0, 0, 0)
    _f.BackgroundTransparency = 0.2
    _f.Visible = false
    _f.Parent = _b

    local _vis = false
    _b.MouseButton1Click:Connect(function()
        _vis = not _vis
        _f.Visible = _vis
    end)

    local function _btn(n, x, y, t, cb)
        local _btn = Instance.new("TextButton")
        _btn.Size = UDim2.new(0, 50, 0, 40)
        _btn.BackgroundColor3 = Color3.new(0, 7, 7)
        _btn.Position = UDim2.new(0, x, 0, y)
        _btn.Text = t
        _btn.TextScaled = true
        _btn.Parent = _f
        _btn.MouseButton1Click:Connect(function()
            _btn.BackgroundColor3 = Color3.new(0, 0, 1)
            wait(0.1)
            _btn.BackgroundColor3 = Color3.new(0, 7, 7)
            setclipboard(cb)
        end)
    end

    _btn(1, 20, 20, "Create TextButton", [[local b = Instance.new("TextButton")
b.Size = UDim2.new(0, 50, 0, 40)
b.BackgroundColor3 = Color3.new(0, 7, 7)
b.Position = UDim2.new(0, 20, 0, 20)
b.Text = "Botao"
b.TextScaled = true
b.Parent = coloca o parent]])

    _btn(2, 80, 20, "Create ScreenGui", [[local pg = game.Players.LocalPlayer.PlayerGui
local sc = Instance.new("ScreenGui")
sc.ResetOnSpawn = false
sc.Parent = pg]])

    _btn(3, 140, 20, "Create Frame", [[local fm = Instance.new("Frame")
fm.Size = UDim2.new(0, 200, 0, 180)
fm.Parent = Seu parent aqui]])

    _btn(4, 200, 20, "Create ScrollFrame", [[local sfm = Instance.new("ScrollingFrame")
sfm.Size = UDim2.new(0, 200, 0, 200)
sfm.CanvasSize = UDim2.new(0, 0, 0, 100)
sfm.ScrollBarThicknees = 10
sfm.Parent = Seu Parent]])

    local _ui = Instance.new("UIStroke")
    _ui.Thickness = 3
    _ui.Color = Color3.new(0, 0, 1)
    _ui.Parent = _f

    _btn(5, 20, 70, "Create TextBox", [[local tbx = Instance.new("TextBox")
tbx.Size = UDim2.new(0, 200, 0, 40)
tbx.Parent = seu Parent]])

    _btn(6, 80, 70, "Create UICorner", [[local uic1 = Instance.new("UICorner")
uic1.Radius = UDim.new(0, 8)
uic1.Parent = seu Parent]])

    _btn(7, 140, 70, "Create UIStroke", [[local uik1 = Instance.new("UIStroke")
uik1.Thickness = 3
uik1.Parent = Seu Parent]])
end

if _wl[_plr.Name] then
    _Fx()
end