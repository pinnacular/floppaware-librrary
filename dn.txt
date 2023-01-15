function library:New(name)
	local menu = {}
	local floppa = Instance.new("ScreenGui")
	local Menu = Instance.new("ImageLabel")
	local TextLabel = Instance.new("TextLabel")
	local TabButtons = Instance.new("Frame")
	local UIListLayout = Instance.new("UIListLayout")
	local Tabs = Instance.new("Frame")
	local UIGradient = Instance.new("UIGradient")
	local gradient = Instance.new("Frame")
	local UIGradient_2 = Instance.new("UIGradient")
	local gradient2 = Instance.new("Frame")
	local UIGradient_3 = Instance.new("UIGradient")
	floppa.Name = "AshleyWasHere"
	floppa.ResetOnSpawn = false;
	floppa.ZIndexBehavior = "Global"
	floppa.DisplayOrder = 420133769;
	local but = Instance.new("TextButton")
	but.Modal = true;
	but.Text = ""
	but.BackgroundTransparency = 1;
	but.Parent = floppa;
	local cursor = Instance.new("ImageLabel")
	cursor.Name = "cursor"
	cursor.Parent = floppa;
	cursor.BackgroundTransparency = 1;
	cursor.Size = UDim2.new(0, 64, 0, 64)
	cursor.Image = "rbxassetid://7543116323"
	cursor.ZIndex = 1000;
	cursor.ImageColor3 = Color3.fromRGB(255, 255, 255)
	local Players = game:GetService("Players")
	local LocalPlayer = Players.LocalPlayer;
	local Mouse = LocalPlayer:GetMouse()
	game:GetService("RunService").RenderStepped:connect(function()
		cursor.Visible = floppa.Enabled;
		cursor.Position = UDim2.new(0, Mouse.X - 32, 0, Mouse.Y - 28)
	end)
	local L_234_ = Instance.new("ScreenGui")
	do
		local L_239_ = Instance.new("TextLabel")
		local L_240_ = Instance.new("Frame")
		local L_241_ = Instance.new("UIListLayout")
		L_234_.Name = "KeybindList"
		L_234_.ZIndexBehavior = Enum.ZIndexBehavior.Global;
		L_234_.Enabled = false;
		L_239_.Parent = L_234_;
		L_239_.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
		L_239_.BorderColor3 = Color3.fromRGB(145, 23, 195)
		L_239_.Position = UDim2.new(0, 1, 0.300000012, 0)
		L_239_.Size = UDim2.new(0, 200, 0, 20)
		L_239_.ZIndex = 2;
		L_239_.Font = Enum.Font.SourceSans;
		L_239_.Text = "keybinds"
		L_239_.TextColor3 = Color3.fromRGB(255, 255, 255)
		L_239_.TextSize = 14.000;
		L_240_.Parent = L_239_;
		L_240_.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		L_240_.BackgroundTransparency = 1.000;
		L_240_.Position = UDim2.new(0, 0, 1, 1)
		L_240_.Size = UDim2.new(1, 0, 1, 0)
		L_241_.Parent = L_240_;
		L_241_.HorizontalAlignment = Enum.HorizontalAlignment.Center;
		L_241_.SortOrder = Enum.SortOrder.LayoutOrder;
		L_234_.Parent = game.CoreGui
	end;
	function keybindadd(L_242_arg0)
		if not L_234_.TextLabel.Frame:FindFirstChild(L_242_arg0) then
			local L_243_ = Instance.new("TextLabel")
			L_243_.BackgroundColor3 = Color3.fromRGB(1, 1, 1)
			L_243_.BackgroundTransparency = 1.000;
			L_243_.BorderColor3 = Color3.fromRGB(145, 23, 195)
			L_243_.BorderSizePixel = 1;
			L_243_.Size = UDim2.new(0, 200, 0, 20)
			L_243_.ZIndex = 2;
			L_243_.Font = Enum.Font.SourceSans;
			L_243_.Text = L_242_arg0;
			L_243_.TextColor3 = Color3.fromRGB(255, 255, 255)
			L_243_.TextSize = 14.000;
			L_243_.TextStrokeTransparency = 0;
			L_243_.Name = L_242_arg0;
			L_243_.Parent = L_234_.TextLabel.Frame
		end
	end;
	function keybindremove(L_244_arg0)
		if L_234_.TextLabel.Frame:FindFirstChild(L_244_arg0) then
			L_234_.TextLabel.Frame:FindFirstChild(L_244_arg0):Destroy()
		end
	end;
	function library:SetKeybindVisible(L_245_arg0)
		L_234_.Enabled = L_245_arg0
	end;
	Menu.Name = "Menu"
	Menu.Parent = floppa;
	Menu.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Menu.BorderSizePixel = 0;
	Menu.Position = UDim2.new(0.5, -300, 0.5, -300)
	Menu.Size = UDim2.new(0, 578, 0, 600)
	Menu.Image = "rbxassetid://8702626168"
	gradient.Name = "gradient"
	gradient.Parent = Menu;
	gradient.Position = UDim2.new(0.022, 0, 0.035, 0)
	gradient.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	gradient.BorderSizePixel = 0;
	gradient.Position = UDim2.new(0.019, 0, 0.031, 0)
	gradient.Size = UDim2.new(0, 554, 0, 2)
	UIGradient_2.Color = ColorSequence.new{
		ColorSequenceKeypoint.new(0.00, Color3.fromRGB(124, 81, 149)),
		ColorSequenceKeypoint.new(0.50, Color3.fromRGB(109, 57, 142)),
		ColorSequenceKeypoint.new(1.00, Color3.fromRGB(79, 48, 112))
	}
	UIGradient_2.Rotation = 90;
	UIGradient_2.Parent = gradient;
	gradient2.Name = "gradient"
	gradient2.Parent = Menu;
	gradient2.Position = UDim2.new(0, 0, 0, 0)
	gradient2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	gradient2.BorderSizePixel = 0;
	gradient2.Position = UDim2.new(0, 2, 0, 596)
	gradient2.Size = UDim2.new(0, 574, 0, 2)
	UIGradient_3.Color = ColorSequence.new{
		ColorSequenceKeypoint.new(0.00, Color3.fromRGB(124, 81, 149)),
		ColorSequenceKeypoint.new(0.50, Color3.fromRGB(109, 57, 142)),
		ColorSequenceKeypoint.new(1.00, Color3.fromRGB(79, 48, 112))
	}
	UIGradient_3.Rotation = 90;
	UIGradient_3.Parent = gradient2;
	TextLabel.Position = UDim2.new(0, 18, 18, 16)
	library.uiopen = true;
	game:GetService("UserInputService").InputBegan:Connect(function(key)
		if key.KeyCode == Enum.KeyCode.Insert or key.KeyCode == Enum.KeyCode.Delete then
			floppa.Enabled = not floppa.Enabled;
			library.uiopen = floppa.Enabled
		end
	end)
	library.dragging = false;
	do
		local UserInputService = game:GetService("UserInputService")
		local a = Menu;
		local dragInput;
		local dragStart;
		local startPos;
		local function update(input)
			local delta = input.Position - dragStart;
			a.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
		end;
		a.InputBegan:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
				library.dragging = true;
				dragStart = input.Position;
				startPos = a.Position;
				input.Changed:Connect(function()
					if input.UserInputState == Enum.UserInputState.End then
						library.dragging = false
					end
				end)
			end
		end)
		a.InputChanged:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
				dragInput = input
			end
		end)
		UserInputService.InputChanged:Connect(function(input)
			if input == dragInput and library.dragging then
				update(input)
			end
		end)
	end;
	TextLabel.Name = name;
	TextLabel.Parent = Menu;
	TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel.BackgroundTransparency = 1.000;
	TextLabel.Position = UDim2.new(0.0119792828, 0, 0, 2)
	TextLabel.Size = UDim2.new(0, 564, 0, 14)
	TextLabel.Font = Enum.Font.Ubuntu;
	TextLabel.Text = name;
	TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel.TextSize = 12.000;
	TextLabel.TextStrokeTransparency = 0.000;
	TextLabel.TextWrapped = true;
	TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
	TabButtons.Name = "TabButtons"
	TabButtons.Parent = Menu;
	TabButtons.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TabButtons.BorderColor3 = Color3.fromRGB(255, 25, 5255)
	TabButtons.BorderSizePixel = 0;
	TabButtons.Position = UDim2.new(0, 11, 0, 23)
	TabButtons.Size = UDim2.new(0, 554, 0, 31)
	UIGradient.Color = ColorSequence.new{
		ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 48)),
		ColorSequenceKeypoint.new(0.96, Color3.fromRGB(31, 31, 31)),
		ColorSequenceKeypoint.new(1.00, Color3.fromRGB(31, 31, 31))
	}
	UIGradient.Rotation = 90;
	UIGradient.Parent = TabButtons;
	UIListLayout.Parent = TabButtons;
	UIListLayout.FillDirection = Enum.FillDirection.Horizontal;
	UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
	Tabs.Name = "Tabs"
	Tabs.Parent = Menu;
	Tabs.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
	Tabs.BackgroundTransparency = 1.000;
	Tabs.Position = UDim2.new(0, -9, 0, 58)
	Tabs.Size = UDim2.new(0, 600, 0, 528)
	local first = true;
	local currenttab;
	function menu:Tab(text)
		local tabname;
		tabname = text;
		local Tab = {}
		values[tabname] = {}
		local TextButton = Instance.new("TextButton")
		TextButton.Parent = TabButtons;
		TextButton.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
		TextButton.BorderColor3 = Color3.fromRGB(20, 20, 20)
		TextButton.BorderSizePixel = 2;
		TextButton.AutoButtonColor = false;
		TextButton.Text = text;
		TextButton.Size = UDim2.new(0, 92, 0, 31)
		TextButton.Font = Enum.Font.Ubuntu;
		TextButton.TextColor3 = Color3.fromRGB(255, 255, 255)
		TextButton.TextSize = 12.000;
		TextButton.TextStrokeTransparency = 0.000;
		local TabGui = Instance.new("ScrollingFrame")
		local Left = Instance.new("ScrollingFrame")
		local UIListLayout = Instance.new("UIListLayout")
		local Right = Instance.new("ScrollingFrame")
		local UIListLayout_2 = Instance.new("UIListLayout")
		TabGui.Name = "TabGui"
		TabGui.Parent = Tabs;
		TabGui.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		TabGui.BackgroundTransparency = 1.000;
		TabGui.Size = UDim2.new(1, 0, 1, 0)
		TabGui.Visible = false;
		TabGui.ScrollBarThickness = 0;
		Left.Name = "Left"
		Left.Parent = TabGui;
		Left.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Left.BackgroundTransparency = 1.000;
		Left.Position = UDim2.new(0, 15, 0, 11)
		Left.Size = UDim2.new(0, 279, 0, 543)
		Left.ScrollBarThickness = 0;
		UIListLayout.Parent = Left;
		UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
		UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
		UIListLayout.Padding = UDim.new(0, 10)
		Right.Name = "Right"
		Right.Parent = TabGui;
		Right.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Right.BackgroundTransparency = 1.000;
		Right.Position = UDim2.new(0, 303, 0, 11)
		Right.Size = UDim2.new(0, 279, 0, 543)
		Right.ScrollBarThickness = 0;
		UIListLayout_2.Parent = Right;
		UIListLayout_2.HorizontalAlignment = Enum.HorizontalAlignment.Center;
		UIListLayout_2.SortOrder = Enum.SortOrder.LayoutOrder;
		UIListLayout_2.Padding = UDim.new(0, 10)
		if first then
			TextButton.TextColor3 = Color3.fromRGB(255, 255, 255)
			currenttab = text;
			TabGui.Visible = true;
			first = false
		end;
		TextButton.MouseButton1Down:Connect(function()
			if currenttab ~= text then
				for i, v in pairs(TabButtons:GetChildren()) do
					if v:IsA("TextButton") then
						library:Tween(v, TweenInfo.new(0.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
							BackgroundTransparency = 0
						})
					end
				end;
				for i, v in pairs(Tabs:GetChildren()) do
					v.Visible = false
				end;
				library:Tween(TextButton, TweenInfo.new(0.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
					BackgroundTransparency = 1
				})
				currenttab = text;
				TabGui.Visible = true
			end
		end)
		function Tab:MSector(text, side)
			local sectorname = text;
			local MSector = {}
			values[tabname][text] = {}
			local Section = Instance.new("Frame")
			local SectionText = Instance.new("TextLabel")
			local Inner = Instance.new("Frame")
			local sectiontabs = Instance.new("Frame")
			local UIListLayout_2 = Instance.new("UIListLayout")
			local gradient = Instance.new("Frame")
			local UIGradient_2 = Instance.new("UIGradient")
			Section.Name = "Section"
			Section.Parent = TabGui[side]
			Section.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
			Section.BackgroundTransparency = 1.000;
			Section.BorderColor3 = Color3.fromRGB(18, 18, 16)
			Section.BorderSizePixel = 0;
			Section.Size = UDim2.new(1, 0, 0, 33)
			SectionText.Name = "SectionText"
			SectionText.Parent = Section;
			SectionText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			SectionText.BackgroundTransparency = 1.000;
			SectionText.Position = UDim2.new(0, 7, 0, -4)
			SectionText.Size = UDim2.new(0, 270, 0, 19)
			SectionText.ZIndex = 2;
			SectionText.Font = Enum.Font.Ubuntu;
			SectionText.TextStrokeTransparency = 0.000;
			SectionText.Text = text;
			SectionText.TextColor3 = Color3.fromRGB(255, 255, 255)
			SectionText.TextSize = 12.000;
			SectionText.TextXAlignment = Enum.TextXAlignment.Left;
			Inner.Name = "Inner"
			Inner.Parent = Section;
			Inner.BackgroundColor3 = Color3.fromRGB(31, 31, 31)
			Inner.BackgroundTransparency = 0.000;
			Inner.BorderColor3 = Color3.fromRGB(18, 18, 16)
			Inner.BorderSizePixel = 2;
			Inner.Position = UDim2.new(0, 1, 0, 1)
			Inner.Size = UDim2.new(1, -2, 1, -9)
			gradient.Name = "gradient"
			gradient.Parent = Section;
			gradient.Position = UDim2.new(0.022, 0, 0.035, 0)
			gradient.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			gradient.BorderSizePixel = 0;
			gradient.Position = UDim2.new(0, 0, 0, -3)
			gradient.Size = UDim2.new(0, 280, 0, 2)
			UIGradient_2.Color = ColorSequence.new{
				ColorSequenceKeypoint.new(0.00, Color3.fromRGB(124, 81, 149)),
				ColorSequenceKeypoint.new(0.50, Color3.fromRGB(109, 57, 142)),
				ColorSequenceKeypoint.new(1.00, Color3.fromRGB(79, 48, 112))
			}
			UIGradient_2.Rotation = 90;
			UIGradient_2.Parent = gradient;
			sectiontabs.Name = "sectiontabs"
			sectiontabs.Parent = Section;
			sectiontabs.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			sectiontabs.BackgroundTransparency = 1.000;
			sectiontabs.Position = UDim2.new(0, 0, 0, 6)
			sectiontabs.Size = UDim2.new(1, 0, 0, 22)
			UIListLayout_2.Parent = sectiontabs;
			UIListLayout_2.FillDirection = Enum.FillDirection.Horizontal;
			UIListLayout_2.HorizontalAlignment = Enum.HorizontalAlignment.Center;
			UIListLayout_2.SortOrder = Enum.SortOrder.LayoutOrder;
			UIListLayout_2.Padding = UDim.new(0, 2)
			local firs = true;
			local selected;
			function MSector:Tab(text)
				local tab = {}
				values[tabname][sectorname][text] = {}
				local tabtext = text;
				local tabsize = UDim2.new(1, 0, 0, 44)
				local tab1 = Instance.new("Frame")
				local UIPadding = Instance.new("UIPadding")
				local UIListLayout = Instance.new("UIListLayout")
				local TextButton = Instance.new("TextButton")
				tab1.Name = text;
				tab1.Parent = Inner;
				tab1.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
				tab1.BorderColor3 = Color3.fromRGB(18, 18, 16)
				tab1.BorderSizePixel = 0;
				tab1.BackgroundTransparency = 1.000;
				tab1.Position = UDim2.new(0, 0, 0, 30)
				tab1.Size = UDim2.new(1, 0, 1, -21)
				tab1.Name = text;
				tab1.Visible = false;
				UIPadding.Parent = tab1;
				UIPadding.PaddingTop = UDim.new(0, 0)
				UIListLayout.Parent = tab1;
				UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
				UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
				UIListLayout.Padding = UDim.new(0, 0)
				TextButton.Parent = sectiontabs;
				TextButton.BackgroundColor3 = Color3.fromRGB(23, 23, 23)
				TextButton.BorderColor3 = Color3.fromRGB(23, 23, 23)
				TextButton.BackgroundTransparency = 1.000;
				TextButton.Size = UDim2.new(0, txt:GetTextSize(text, 14, Enum.Font.Ubuntu, Vector2.new(700, 700)).X + 0, 1, 0)
				TextButton.Font = Enum.Font.Ubuntu;
				TextButton.Text = text;
				TextButton.TextStrokeTransparency = 0.000;
				TextButton.TextColor3 = Color3.fromRGB(255, 255, 255)
				TextButton.TextSize = 10.000;
				TextButton.Name = text;
				TextButton.MouseButton1Down:Connect(function()
					for i, v in pairs(Inner:GetChildren()) do
						v.Visible = false
					end;
					for i, v in pairs(sectiontabs:GetChildren()) do
						if v:IsA('TextButton') then
							library:Tween(v, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end
					end;
					Section.Size = tabsize;
					tab1.Visible = true;
					library:Tween(TextButton, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
						TextColor3 = Color3.fromRGB(109, 57, 142)
					})
				end)
				function tab:Element(type, text, data, callback)
					local Element = {}
					data = data or {}
					callback = callback or function()
					end;
					values[tabname][sectorname][tabtext][text] = {}
					if type == "Jumbobox" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 39)
						Element.value = {
							Jumbobox = {}
						}
						data.options = data.options or {}
						local Dropdown = Instance.new("Frame")
						local Button = Instance.new("TextButton")
						local TextLabel = Instance.new("TextLabel")
						local Drop = Instance.new("ScrollingFrame")
						local Button_2 = Instance.new("TextButton")
						local TextLabel_2 = Instance.new("TextLabel")
						local UIListLayout = Instance.new("UIListLayout")
						local ImageLabel = Instance.new("ImageLabel")
						local TextLabel_3 = Instance.new("TextLabel")
						Dropdown.Name = "Dropdown"
						Dropdown.Parent = tab1;
						Dropdown.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Dropdown.BackgroundTransparency = 1.000;
						Dropdown.Position = UDim2.new(0, 0, 0.255102038, 0)
						Dropdown.Size = UDim2.new(1, 0, 0, 39)
						Button.Name = "Button"
						Button.Parent = Dropdown;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Button.Position = UDim2.new(0, 30, 0, 16)
						Button.Size = UDim2.new(0, 175, 0, 17)
						Button.AutoButtonColor = false;
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(255, 255, 255)
						Button.TextSize = 10.000;
						local UIGradient = Instance.new("UIGradient")
						UIGradient.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
							ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
						}
						UIGradient.Rotation = 90;
						UIGradient.Parent = Button;
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
						TextLabel.Position = UDim2.new(0, 5, 0, 0)
						TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = "-"
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						local abcd = TextLabel;
						Drop.Name = "Drop"
						Drop.Parent = Button;
						Drop.Active = true;
						Drop.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Drop.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Drop.Position = UDim2.new(0, 0, 1, 1)
						Drop.Size = UDim2.new(1, 0, 0, 20)
						Drop.Visible = false;
						Drop.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
						Drop.CanvasSize = UDim2.new(1, 1, 1, 1)
						Drop.ScrollBarThickness = 0;
						Drop.TopImage = "http://www.roblox.com/asset/?id=6724808282"
						Drop.MidImage = "http://www.roblox.com/asset/?id=6724808282"
						Drop.AutomaticCanvasSize = "Y"
						Drop.ZIndex = 5;
						Drop.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
						UIListLayout.Parent = Drop;
						UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
						UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
						values[tabname][sectorname][tabtext][text] = Element.value;
						local num = #data.options;
						if num > 5 then
							Drop.Size = UDim2.new(1, 0, 0, 85)
						else
							Drop.Size = UDim2.new(1, 0, 0, 17 * num)
						end;
						local first = true;
						local function updatetext()
							local old = {}
							for i, v in ipairs(data.options) do
								if table.find(Element.value.Jumbobox, v) then
									table.insert(old, v)
								else
								end
							end;
							local str = ""
							if #old == 0 then
								str = "..."
							else
								if #old == 1 then
									str = old[1]
								else
									for i, v in ipairs(old) do
										if i == 1 then
											str = v
										else
											if i > 2 then
												if i < 4 then
													str = str .. ",  ..."
												end
											else
												str = str .. ",  " .. v
											end
										end
									end
								end
							end;
							abcd.Text = str
						end;
						for i, v in ipairs(data.options) do
							do
								local Button = Instance.new("TextButton")
								local TextLabel = Instance.new("TextLabel")
								Button.Name = v;
								Button.Parent = Drop;
								Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
								Button.Position = UDim2.new(0, 30, 0, 16)
								Button.Size = UDim2.new(0, 175, 0, 17)
								Button.AutoButtonColor = false;
								Button.Font = Enum.Font.Ubuntu;
								Button.Text = ""
								Button.TextColor3 = Color3.fromRGB(255, 255, 255)
								Button.TextSize = 10.000;
								Button.BorderSizePixel = 0;
								Button.ZIndex = 6;
								TextLabel.Parent = Button;
								TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
								TextLabel.BackgroundTransparency = 1.000;
								TextLabel.BorderColor3 = Color3.fromRGB(25, 25, 25)
								TextLabel.Position = UDim2.new(0, 5, 0, -1)
								TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
								TextLabel.Font = Enum.Font.Ubuntu;
								TextLabel.Text = v;
								TextLabel.TextStrokeTransparency = 0.000;
								TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
								TextLabel.TextSize = 10.000;
								TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
								TextLabel.ZIndex = 6;
								Button.MouseButton1Down:Connect(function()
									if table.find(Element.value.Jumbobox, v) then
										for i, a in pairs(Element.value.Jumbobox) do
											if a == v then
												table.remove(Element.value.Jumbobox, i)
											end
										end;
										library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(255, 255, 255)
										})
									else
										table.insert(Element.value.Jumbobox, v)
										library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(255, 255, 255)
										})
									end;
									updatetext()
									values[tabname][sectorname][tabtext][text] = Element.value;
									callback(Element.value)
								end)
								Button.MouseEnter:Connect(function()
									if not table.find(Element.value.Jumbobox, v) then
										library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(255, 255, 255)
										})
									end
								end)
								Button.MouseLeave:Connect(function()
									if not table.find(Element.value.Jumbobox, v) then
										library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(255, 255, 255)
										})
									end
								end)
								first = false
							end
						end;
						function Element:SetValue(val)
							Element.value = val;
							for i, v in pairs(Drop:GetChildren()) do
								if v.Name ~= "UIListLayout" then
									if table.find(val.Jumbobox, v.Name) then
										v.TextLabel.TextColor3 = Color3.fromRGB(109, 57, 142)
									else
										v.TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
									end
								end
							end;
							updatetext()
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(val)
						end;
						if data.default then
							Element:SetValue(data.default)
						end;
						ImageLabel.Parent = Button;
						ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						ImageLabel.BackgroundTransparency = 1.000;
						ImageLabel.Position = UDim2.new(0, 165, 0, 6)
						ImageLabel.Size = UDim2.new(0, 6, 0, 4)
						ImageLabel.Image = "http://www.roblox.com/asset/?id=6724771531"
						TextLabel_3.Parent = Dropdown;
						TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel_3.BackgroundTransparency = 1.000;
						TextLabel_3.Position = UDim2.new(0, 32, 0, -1)
						TextLabel_3.Size = UDim2.new(0.111913361, 208, 0.382215232, 0)
						TextLabel_3.Font = Enum.Font.Ubuntu;
						TextLabel_3.Text = text;
						TextLabel_3.TextStrokeTransparency = 0.000;
						TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel_3.TextSize = 10.000;
						TextLabel_3.TextXAlignment = Enum.TextXAlignment.Left;
						Button.MouseButton1Down:Connect(function()
							Drop.Visible = not Drop.Visible;
							if not Drop.Visible then
								Drop.CanvasPosition = Vector2.new(0, 0)
							end
						end)
						local indrop = false;
						local ind = false;
						Drop.MouseEnter:Connect(function()
							indrop = true
						end)
						Drop.MouseLeave:Connect(function()
							indrop = false
						end)
						Button.MouseEnter:Connect(function()
							ind = true
						end)
						Button.MouseLeave:Connect(function()
							ind = false
						end)
						game:GetService("UserInputService").InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
								if Drop.Visible == true and not indrop and not ind then
									Drop.Visible = false;
									Drop.CanvasPosition = Vector2.new(0, 0)
								end
							end
						end)
					elseif type == "TextBox" then
					elseif type == "ToggleKeybind" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 16)
						Element.value = {
							Toggle = data.default and data.default.Toggle or false,
							Key,
							Type = "Always",
							Active = true
						}
						local Toggle = Instance.new("Frame")
						local Button = Instance.new("TextButton")
						local Color = Instance.new("Frame")
						local TextLabel = Instance.new("TextLabel")
						Toggle.Name = "Toggle"
						Toggle.Parent = tab1;
						Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Toggle.BackgroundTransparency = 1.000;
						Toggle.Size = UDim2.new(1, 0, 0, 15)
						Button.Name = "Button"
						Button.Parent = Toggle;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BackgroundTransparency = 1.000;
						Button.Size = UDim2.new(1, 0, 1, 0)
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						Color.Name = "Color"
						Color.Parent = Button;
						Color.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Color.Position = UDim2.new(0, 15, 0.5, -5)
						Color.Size = UDim2.new(0, 8, 0, 8)
						local binding = false;
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.Position = UDim2.new(0, 32, 0, -1)
						TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = text;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						local function update()
							if Element.value.Toggle then
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(109, 57, 142)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							else
								keybindremove(text)
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end;
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end;
						Button.MouseButton1Down:Connect(function()
							if not binding then
								Element.value.Toggle = not Element.value.Toggle;
								update()
								values[tabname][sectorname][tabtext][text] = Element.value;
								callback(Element.value)
							end
						end)
						if data.default then
							update()
						end;
						values[tabname][sectorname][tabtext][text] = Element.value;
						do
							local Keybind = Instance.new("TextButton")
							local Frame = Instance.new("Frame")
							local Always = Instance.new("TextButton")
							local UIListLayout = Instance.new("UIListLayout")
							local Hold = Instance.new("TextButton")
							local Toggle = Instance.new("TextButton")
							Keybind.Name = "Keybind"
							Keybind.Parent = Button;
							Keybind.BackgroundColor3 = Color3.fromRGB(23, 23, 23)
							Keybind.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Keybind.Position = UDim2.new(0, 270, 0.5, -6)
							Keybind.Text = "none"
							Keybind.BackgroundTransparency = 1.000;
							Keybind.Size = UDim2.new(0, 43, 0, 12)
							Keybind.Size = UDim2.new(0, txt:GetTextSize("none", 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 5, 0, 12)
							Keybind.AutoButtonColor = false;
							Keybind.Font = Enum.Font.Ubuntu;
							Keybind.TextColor3 = Color3.fromRGB(255, 255, 255)
							Keybind.TextSize = 10.000;
							Keybind.AnchorPoint = Vector2.new(1, 0)
							Keybind.ZIndex = 3;
							Frame.Parent = Keybind;
							Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Frame.Position = UDim2.new(1, -49, 0, 1)
							Frame.Size = UDim2.new(0, 49, 0, 49)
							Frame.Visible = false;
							Frame.ZIndex = 3;
							Always.Name = "Always"
							Always.Parent = Frame;
							Always.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Always.BackgroundTransparency = 1.000;
							Always.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Always.Position = UDim2.new(-3.03289485, 231, 0.115384616, -6)
							Always.Size = UDim2.new(1, 0, 0, 16)
							Always.AutoButtonColor = false;
							Always.Font = Enum.Font.Ubuntu;
							Always.Text = "Always"
							Always.TextStrokeTransparency = 0.000;
							Always.TextColor3 = Color3.fromRGB(109, 57, 142)
							Always.TextSize = 10.000;
							Always.ZIndex = 3;
							UIListLayout.Parent = Frame;
							UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
							UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
							Hold.Name = "Hold"
							Hold.Parent = Frame;
							Hold.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Hold.BackgroundTransparency = 1.000;
							Hold.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Hold.Position = UDim2.new(-3.03289485, 231, 0.115384616, -6)
							Hold.Size = UDim2.new(1, 0, 0, 16)
							Hold.TextStrokeTransparency = 0.000;
							Hold.AutoButtonColor = false;
							Hold.Font = Enum.Font.Ubuntu;
							Hold.Text = "Hold"
							Hold.TextColor3 = Color3.fromRGB(255, 255, 255)
							Hold.TextSize = 10.000;
							Hold.ZIndex = 3;
							Toggle.Name = "Toggle"
							Toggle.Parent = Frame;
							Toggle.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Toggle.BackgroundTransparency = 1.000;
							Toggle.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Toggle.Position = UDim2.new(-3.03289485, 231, 0.115384616, -6)
							Toggle.Size = UDim2.new(1, 0, 0, 16)
							Toggle.AutoButtonColor = false;
							Toggle.Font = Enum.Font.Ubuntu;
							Toggle.Text = "Toggle"
							Toggle.TextStrokeTransparency = 0.000;
							Toggle.TextColor3 = Color3.fromRGB(255, 255, 255)
							Toggle.TextSize = 10.000;
							Toggle.ZIndex = 3;
							for _, button in pairs(Frame:GetChildren()) do
								if button:IsA("TextButton") then
									button.MouseButton1Down:Connect(function()
										Element.value.Type = button.Text;
										Frame.Visible = false;
										Element.value.Active = Element.value.Type == "Always" and true or false;
										if Element.value.Type == "Always" then
											keybindremove(text)
										end;
										for _, button in pairs(Frame:GetChildren()) do
											if button:IsA("TextButton") and button.Text ~= Element.value.Type then
												button.Font = Enum.Font.Ubuntu;
												library:Tween(button, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
													TextColor3 = Color3.fromRGB(255, 255, 255)
												})
											end
										end;
										button.Font = Enum.Font.Ubuntu;
										button.TextColor3 = Color3.fromRGB(109, 57, 142)
										values[tabname][sectorname][tabtext][text] = Element.value;
										callback(Element.value)
									end)
									button.MouseEnter:Connect(function()
										if Element.value.Type ~= button.Text then
											library:Tween(button, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
												TextColor3 = Color3.fromRGB(255, 255, 255)
											})
										end
									end)
									button.MouseLeave:Connect(function()
										if Element.value.Type ~= button.Text then
											library:Tween(button, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
												TextColor3 = Color3.fromRGB(255, 255, 255)
											})
										end
									end)
								end
							end;
							Keybind.MouseButton1Down:Connect(function()
								if not binding then
									wait()
									binding = true;
									Keybind.Text = "-"
									Keybind.Size = UDim2.new(0, txt:GetTextSize("-", 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 4, 0, 12)
								end
							end)
							Keybind.MouseButton2Down:Connect(function()
								if not binding then
									Frame.Visible = not Frame.Visible
								end
							end)
							local Player = game.Players.LocalPlayer;
							local Mouse = Player:GetMouse()
							local InFrame = false;
							Frame.MouseEnter:Connect(function()
								InFrame = true
							end)
							Frame.MouseLeave:Connect(function()
								InFrame = false
							end)
							local InFrame2 = false;
							Keybind.MouseEnter:Connect(function()
								InFrame2 = true
							end)
							Keybind.MouseLeave:Connect(function()
								InFrame2 = false
							end)
							game:GetService("UserInputService").InputBegan:Connect(function(input)
								if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 and not binding then
									if Frame.Visible == true and not InFrame and not InFrame2 then
										Frame.Visible = false
									end
								end;
								if binding then
									binding = false;
									Keybind.Text = input.KeyCode.Name ~= "Unknown" and input.KeyCode.Name:upper() or input.UserInputType.Name:upper()
									Keybind.Size = UDim2.new(0, txt:GetTextSize(Keybind.Text, 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 5, 0, 12)
									Element.value.Key = input.KeyCode.Name ~= "Unknown" and input.KeyCode.Name or input.UserInputType.Name;
									if input.KeyCode.Name == "Backspace" then
										Keybind.Text = "none"
										Keybind.Size = UDim2.new(0, txt:GetTextSize(Keybind.Text, 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 4, 0, 12)
										Element.value.Key = nil
									end
								else
									if Element.value.Key ~= nil then
										if string.find(Element.value.Key, "Mouse") then
											if input.UserInputType == Enum.UserInputType[Element.value.Key] then
												if Element.value.Type == "Hold" then
													Element.value.Active = true;
													if Element.value.Active and Element.value.Toggle then
														keybindhold(text)
													else
														keybindremove(text)
													end
												elseif Element.value.Type == "Toggle" then
													Element.value.Active = not Element.value.Active;
													if Element.value.Active and Element.value.Toggle then
														keybindadd(text)
													else
														keybindremove(text)
													end
												end
											end
										else
											if input.KeyCode == Enum.KeyCode[Element.value.Key] then
												if Element.value.Type == "Hold" then
													Element.value.Active = true;
													if Element.value.Active and Element.value.Toggle then
														keybindhold(text)
													else
														keybindremove(text)
													end
												elseif Element.value.Type == "Toggle" then
													Element.value.Active = not Element.value.Active;
													if Element.value.Active and Element.value.Toggle then
														keybindadd(text)
													else
														keybindremove(text)
													end
												end
											end
										end
									else
										Element.value.Active = true
									end
								end;
								values[tabname][sectorname][tabtext][text] = Element.value;
								callback(Element.value)
							end)
							game:GetService("UserInputService").InputEnded:Connect(function(input)
								if Element.value.Key ~= nil then
									if string.find(Element.value.Key, "Mouse") then
										if input.UserInputType == Enum.UserInputType[Element.value.Key] then
											if Element.value.Type == "Hold" then
												Element.value.Active = false;
												if Element.value.Active and Element.value.Toggle then
													keybindadd(text)
												else
													keybindremove(text)
												end
											end
										end
									else
										if input.KeyCode == Enum.KeyCode[Element.value.Key] then
											if Element.value.Type == "Hold" then
												Element.value.Active = false;
												if Element.value.Active and Element.value.Toggle then
													keybindhold(text)
												else
													keybindremove(text)
												end
											end
										end
									end
								end;
								values[tabname][sectorname][tabtext][text] = Element.value;
								callback(Element.value)
							end)
						end;
						function Element:SetValue(value)
							Element.value = value;
							update()
						end
					elseif type == "Toggle" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 16)
						Element.value = {
							Toggle = data.default and data.default.Toggle or false
						}
						local Toggle = Instance.new("Frame")
						local Button = Instance.new("TextButton")
						local Color = Instance.new("Frame")
						local TextLabel = Instance.new("TextLabel")
						Toggle.Name = "Toggle"
						Toggle.Parent = tab1;
						Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Toggle.BackgroundTransparency = 1.000;
						Toggle.Size = UDim2.new(1, 0, 0, 15)
						Button.Name = "Button"
						Button.Parent = Toggle;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BackgroundTransparency = 1.000;
						Button.Size = UDim2.new(1, 0, 1, 0)
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						Color.Name = "Color"
						Color.Parent = Button;
						Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Color.Position = UDim2.new(0, 15, 0.5, -5)
						Color.Size = UDim2.new(0, 8, 0, 8)
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.Position = UDim2.new(0, 32, 0, -1)
						TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = text;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						local function update()
							if Element.value.Toggle then
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(109, 57, 142)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							else
								keybindremove(text)
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end;
							values[tabname][sectorname][tabtext][text] = Element.value
						end;
						Button.MouseButton1Down:Connect(function()
							Element.value.Toggle = not Element.value.Toggle;
							update()
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end)
						if data.default then
							update()
						end;
						values[tabname][sectorname][tabtext][text] = Element.value;
						function Element:SetValue(value)
							Element.value = value;
							values[tabname][sectorname][tabtext][text] = Element.value;
							update()
							callback(Element.value)
						end
					elseif type == "ToggleColor" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 16)
						Element.value = {
							Toggle = data.default and data.default.Toggle or false,
							Color = data.default and data.default.Color or Color3.fromRGB(255, 255, 255)
						}
						local Toggle = Instance.new("Frame")
						local Button = Instance.new("TextButton")
						local Color = Instance.new("Frame")
						local TextLabel = Instance.new("TextLabel")
						Toggle.Name = "Toggle"
						Toggle.Parent = tab1;
						Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Toggle.BackgroundTransparency = 1.000;
						Toggle.Size = UDim2.new(1, 0, 0, 15)
						Button.Name = "Button"
						Button.Parent = Toggle;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BackgroundTransparency = 1.000;
						Button.Size = UDim2.new(1, 0, 1, 0)
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						Color.Name = "Color"
						Color.Parent = Button;
						Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Color.Position = UDim2.new(0, 15, 0.5, -5)
						Color.Size = UDim2.new(0, 8, 0, 8)
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.Position = UDim2.new(0, 32, 0, -1)
						TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = text;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						local function update()
							if Element.value.Toggle then
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(109, 57, 142)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							else
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end;
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end;
						local ColorH, ColorS, ColorV;
						local ColorP = Instance.new("TextButton")
						local Frame = Instance.new("Frame")
						local Colorpick = Instance.new("ImageButton")
						local ColorDrag = Instance.new("Frame")
						local Huepick = Instance.new("ImageButton")
						local Huedrag = Instance.new("Frame")
						ColorP.Name = "ColorP"
						ColorP.Parent = Button;
						ColorP.AnchorPoint = Vector2.new(1, 0)
						ColorP.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
						ColorP.BorderColor3 = Color3.fromRGB(18, 18, 16)
						ColorP.Position = UDim2.new(0, 270, 0.5, -4)
						ColorP.Size = UDim2.new(0, 18, 0, 8)
						ColorP.AutoButtonColor = false;
						ColorP.Font = Enum.Font.Ubuntu;
						ColorP.Text = ""
						ColorP.TextColor3 = Color3.fromRGB(255, 255, 255)
						ColorP.TextSize = 10.000;
						Frame.Parent = ColorP;
						Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Frame.Position = UDim2.new(-0.666666687, -170, 1.375, 0)
						Frame.Size = UDim2.new(0, 200, 0, 170)
						Frame.Visible = false;
						Frame.ZIndex = 3;
						Colorpick.Name = "Colorpick"
						Colorpick.Parent = Frame;
						Colorpick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Colorpick.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Colorpick.ClipsDescendants = false;
						Colorpick.Position = UDim2.new(0, 40, 0, 10)
						Colorpick.Size = UDim2.new(0, 150, 0, 150)
						Colorpick.AutoButtonColor = false;
						Colorpick.Image = "rbxassetid://4155801252"
						Colorpick.ImageColor3 = Color3.fromRGB(255, 0, 0)
						Colorpick.ZIndex = 3;
						ColorDrag.Name = "ColorDrag"
						ColorDrag.Parent = Colorpick;
						ColorDrag.AnchorPoint = Vector2.new(0.5, 0.5)
						ColorDrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						ColorDrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
						ColorDrag.Size = UDim2.new(0, 4, 0, 4)
						ColorDrag.ZIndex = 3;
						Huepick.Name = "Huepick"
						Huepick.Parent = Frame;
						Huepick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Huepick.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Huepick.ClipsDescendants = false;
						Huepick.Position = UDim2.new(0, 10, 0, 10)
						Huepick.Size = UDim2.new(0, 20, 0, 150)
						Huepick.AutoButtonColor = false;
						Huepick.Image = "rbxassetid://3641079629"
						Huepick.ImageColor3 = Color3.fromRGB(255, 0, 0)
						Huepick.ImageTransparency = 1;
						Huepick.BackgroundTransparency = 0;
						Huepick.ZIndex = 3;
						local HueFrameGradient = Instance.new("UIGradient")
						HueFrameGradient.Rotation = 90;
						HueFrameGradient.Name = "HueFrameGradient"
						HueFrameGradient.Parent = Huepick;
						HueFrameGradient.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 0, 0)),
							ColorSequenceKeypoint.new(0.17, Color3.fromRGB(255, 0, 255)),
							ColorSequenceKeypoint.new(0.33, Color3.fromRGB(0, 0, 255)),
							ColorSequenceKeypoint.new(0.50, Color3.fromRGB(0, 255, 255)),
							ColorSequenceKeypoint.new(0.67, Color3.fromRGB(0, 255, 0)),
							ColorSequenceKeypoint.new(0.83, Color3.fromRGB(255, 255, 0)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 0, 0))
						}
						Huedrag.Name = "Huedrag"
						Huedrag.Parent = Huepick;
						Huedrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Huedrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Huedrag.Size = UDim2.new(1, 0, 0, 2)
						Huedrag.ZIndex = 3;
						ColorP.MouseButton1Down:Connect(function()
							Frame.Visible = not Frame.Visible
						end)
						local abc = false;
						local inCP = false;
						ColorP.MouseEnter:Connect(function()
							abc = true
						end)
						ColorP.MouseLeave:Connect(function()
							abc = false
						end)
						Frame.MouseEnter:Connect(function()
							inCP = true
						end)
						Frame.MouseLeave:Connect(function()
							inCP = false
						end)
						ColorH = (math.clamp(Huedrag.AbsolutePosition.Y - Huepick.AbsolutePosition.Y, 0, Huepick.AbsoluteSize.Y) / Huepick.AbsoluteSize.Y)
						ColorS = 1 - (math.clamp(ColorDrag.AbsolutePosition.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
						ColorV = 1 - (math.clamp(ColorDrag.AbsolutePosition.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
						if data.default.Color ~= nil then
							ColorH, ColorS, ColorV = data.default.Color:ToHSV()
							ColorH = math.clamp(ColorH, 0, 1)
							ColorS = math.clamp(ColorS, 0, 1)
							ColorV = math.clamp(ColorV, 0, 1)
							ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
						end;
						local mouse = LocalPlayer:GetMouse()
						game:GetService("UserInputService").InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
								if not dragging and not abc and not inCP then
									Frame.Visible = false
								end
							end
						end)
						local function updateColor()
							local ColorX = (math.clamp(mouse.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
							local ColorY = (math.clamp(mouse.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
							ColorDrag.Position = UDim2.new(ColorX, 0, ColorY, 0)
							ColorS = 1 - ColorX;
							ColorV = 1 - ColorY;
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							values[tabname][sectorname][tabtext][text] = Element.value;
							Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
							callback(Element.value)
						end;
						local function updateHue()
							local y = math.clamp(mouse.Y - Huepick.AbsolutePosition.Y, 0, 148)
							Huedrag.Position = UDim2.new(0, 0, 0, y)
							hue = y / 148;
							ColorH = 1 - hue;
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							values[tabname][sectorname][tabtext][text] = Element.value;
							Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
							callback(Element.value)
						end;
						Colorpick.MouseButton1Down:Connect(function()
							updateColor()
							moveconnection = mouse.Move:Connect(function()
								updateColor()
							end)
							releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
								if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
									updateColor()
									moveconnection:Disconnect()
									releaseconnection:Disconnect()
								end
							end)
						end)
						Huepick.MouseButton1Down:Connect(function()
							updateHue()
							moveconnection = mouse.Move:Connect(function()
								updateHue()
							end)
							releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
								if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
									updateHue()
									moveconnection:Disconnect()
									releaseconnection:Disconnect()
								end
							end)
						end)
						Button.MouseButton1Down:Connect(function()
							Element.value.Toggle = not Element.value.Toggle;
							update()
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end)
						if data.default then
							update()
						end;
						values[tabname][sectorname][tabtext][text] = Element.value;
						function Element:SetValue(value)
							Element.value = value;
							local duplicate = Color3.new(value.Color.R, value.Color.G, value.Color.B)
							ColorH, ColorS, ColorV = duplicate:ToHSV()
							ColorH = math.clamp(ColorH, 0, 1)
							ColorS = math.clamp(ColorS, 0, 1)
							ColorV = math.clamp(ColorV, 0, 1)
							ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							update()
							Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
						end
					elseif type == "ToggleTrans" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 16)
						Element.value = {
							Toggle = data.default and data.default.Toggle or false,
							Color = data.default and data.default.Color or Color3.fromRGB(255, 255, 255),
							Transparency = data.default and data.default.Transparency or 0
						}
						local Toggle = Instance.new("Frame")
						local Button = Instance.new("TextButton")
						local Color = Instance.new("Frame")
						local TextLabel = Instance.new("TextLabel")
						Toggle.Name = "Toggle"
						Toggle.Parent = tab1;
						Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Toggle.BackgroundTransparency = 1.000;
						Toggle.Size = UDim2.new(1, 0, 0, 15)
						Button.Name = "Button"
						Button.Parent = Toggle;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BackgroundTransparency = 1.000;
						Button.Size = UDim2.new(1, 0, 1, 0)
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						Color.Name = "Color"
						Color.Parent = Button;
						Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Color.Position = UDim2.new(0, 15, 0.5, -5)
						Color.Size = UDim2.new(0, 8, 0, 8)
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.Position = UDim2.new(0, 32, 0, -1)
						TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = text;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						local function update()
							if Element.value.Toggle then
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(109, 57, 142)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							else
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								})
								tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									BorderColor3 = Color3.fromRGB(18, 18, 16)
								})
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end;
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end;
						local ColorH, ColorS, ColorV;
						local ColorP = Instance.new("TextButton")
						local Frame = Instance.new("Frame")
						local Colorpick = Instance.new("ImageButton")
						local ColorDrag = Instance.new("Frame")
						local Huepick = Instance.new("ImageButton")
						local Huedrag = Instance.new("Frame")
						ColorP.Name = "ColorP"
						ColorP.Parent = Button;
						ColorP.AnchorPoint = Vector2.new(1, 0)
						ColorP.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
						ColorP.BorderColor3 = Color3.fromRGB(18, 18, 16)
						ColorP.Position = UDim2.new(0, 270, 0.5, -4)
						ColorP.Size = UDim2.new(0, 18, 0, 8)
						ColorP.AutoButtonColor = false;
						ColorP.Font = Enum.Font.Ubuntu;
						ColorP.Text = ""
						ColorP.TextColor3 = Color3.fromRGB(255, 255, 255)
						ColorP.TextSize = 10.000;
						Frame.Parent = ColorP;
						Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Frame.Position = UDim2.new(-0.666666687, -170, 1.375, 0)
						Frame.Size = UDim2.new(0, 200, 0, 190)
						Frame.Visible = false;
						Frame.ZIndex = 3;
						Colorpick.Name = "Colorpick"
						Colorpick.Parent = Frame;
						Colorpick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Colorpick.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Colorpick.ClipsDescendants = false;
						Colorpick.Position = UDim2.new(0, 40, 0, 10)
						Colorpick.Size = UDim2.new(0, 150, 0, 150)
						Colorpick.AutoButtonColor = false;
						Colorpick.Image = "rbxassetid://4155801252"
						Colorpick.ImageColor3 = Color3.fromRGB(255, 0, 0)
						Colorpick.ZIndex = 3;
						ColorDrag.Name = "ColorDrag"
						ColorDrag.Parent = Colorpick;
						ColorDrag.AnchorPoint = Vector2.new(0.5, 0.5)
						ColorDrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						ColorDrag.BorderColor3 = Color3.fromRGB(25, 25, 25)
						ColorDrag.Size = UDim2.new(0, 4, 0, 4)
						ColorDrag.ZIndex = 3;
						Huepick.Name = "Huepick"
						Huepick.Parent = Frame;
						Huepick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Huepick.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Huepick.ClipsDescendants = true;
						Huepick.Position = UDim2.new(0, 10, 0, 10)
						Huepick.Size = UDim2.new(0, 20, 0, 150)
						Huepick.AutoButtonColor = false;
						Huepick.Image = "rbxassetid://3641079629"
						Huepick.ImageColor3 = Color3.fromRGB(255, 0, 0)
						Huepick.ImageTransparency = 1;
						Huepick.BackgroundTransparency = 0;
						Huepick.ZIndex = 3;
						local HueFrameGradient = Instance.new("UIGradient")
						HueFrameGradient.Rotation = 90;
						HueFrameGradient.Name = "HueFrameGradient"
						HueFrameGradient.Parent = Huepick;
						HueFrameGradient.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 0, 0)),
							ColorSequenceKeypoint.new(0.17, Color3.fromRGB(255, 0, 255)),
							ColorSequenceKeypoint.new(0.33, Color3.fromRGB(0, 0, 255)),
							ColorSequenceKeypoint.new(0.50, Color3.fromRGB(0, 255, 255)),
							ColorSequenceKeypoint.new(0.67, Color3.fromRGB(0, 255, 0)),
							ColorSequenceKeypoint.new(0.83, Color3.fromRGB(255, 255, 0)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 0, 0))
						}
						Huedrag.Name = "Huedrag"
						Huedrag.Parent = Huepick;
						Huedrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Huedrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Huedrag.Size = UDim2.new(1, 0, 0, 2)
						Huedrag.ZIndex = 3;
						local Transpick = Instance.new("ImageButton")
						local Transcolor = Instance.new("ImageLabel")
						local Transdrag = Instance.new("Frame")
						Transpick.Name = "Transpick"
						Transpick.Parent = Frame;
						Transpick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Transpick.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Transpick.Position = UDim2.new(0, 10, 0, 167)
						Transpick.Size = UDim2.new(0, 180, 0, 15)
						Transpick.AutoButtonColor = false;
						Transpick.Image = "rbxassetid://3887014957"
						Transpick.ScaleType = Enum.ScaleType.Tile;
						Transpick.TileSize = UDim2.new(0, 10, 0, 10)
						Transpick.ZIndex = 3;
						Transcolor.Name = "Transcolor"
						Transcolor.Parent = Transpick;
						Transcolor.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Transcolor.BackgroundTransparency = 1.000;
						Transcolor.Size = UDim2.new(1, 0, 1, 0)
						Transcolor.Image = "rbxassetid://3887017050"
						Transcolor.ImageColor3 = Color3.fromRGB(255, 0, 4)
						Transcolor.ZIndex = 3;
						Transdrag.Name = "Transdrag"
						Transdrag.Parent = Transcolor;
						Transdrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Transdrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Transdrag.Position = UDim2.new(0, -1, 0, 0)
						Transdrag.Size = UDim2.new(0, 2, 1, 0)
						Transdrag.ZIndex = 3;
						ColorP.MouseButton1Down:Connect(function()
							Frame.Visible = not Frame.Visible
						end)
						local abc = false;
						local inCP = false;
						ColorP.MouseEnter:Connect(function()
							abc = true
						end)
						ColorP.MouseLeave:Connect(function()
							abc = false
						end)
						Frame.MouseEnter:Connect(function()
							inCP = true
						end)
						Frame.MouseLeave:Connect(function()
							inCP = false
						end)
						ColorH = (math.clamp(Huedrag.AbsolutePosition.Y - Huepick.AbsolutePosition.Y, 0, Huepick.AbsoluteSize.Y) / Huepick.AbsoluteSize.Y)
						ColorS = 1 - (math.clamp(ColorDrag.AbsolutePosition.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
						ColorV = 1 - (math.clamp(ColorDrag.AbsolutePosition.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
						if data.default.Color ~= nil then
							ColorH, ColorS, ColorV = data.default.Color:ToHSV()
							ColorH = math.clamp(ColorH, 0, 1)
							ColorS = math.clamp(ColorS, 0, 1)
							ColorV = math.clamp(ColorV, 0, 1)
							ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							Transcolor.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
						end;
						if data.default.Transparency ~= nil then
							Transdrag.Position = UDim2.new(data.default.Transparency, -1, 0, 0)
						end;
						local mouse = LocalPlayer:GetMouse()
						game:GetService("UserInputService").InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
								if not dragging and not abc and not inCP then
									Frame.Visible = false
								end
							end
						end)
						local function updateColor()
							local ColorX = (math.clamp(mouse.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
							local ColorY = (math.clamp(mouse.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
							ColorDrag.Position = UDim2.new(ColorX, 0, ColorY, 0)
							ColorS = 1 - ColorX;
							ColorV = 1 - ColorY;
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							Transcolor.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							values[tabname][sectorname][tabtext][text] = Element.value;
							Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
							callback(Element.value)
						end;
						local function updateHue()
							local y = math.clamp(mouse.Y - Huepick.AbsolutePosition.Y, 0, 148)
							Huedrag.Position = UDim2.new(0, 0, 0, y)
							hue = y / 148;
							ColorH = 1 - hue;
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							Transcolor.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							values[tabname][sectorname][tabtext][text] = Element.value;
							Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
							callback(Element.value)
						end;
						local function updateTrans()
							local x = math.clamp(mouse.X - Transpick.AbsolutePosition.X, 0, 178)
							Transdrag.Position = UDim2.new(0, x, 0, 0)
							Element.value.Transparency = (x / 178)
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end;
						Transpick.MouseButton1Down:Connect(function()
							updateTrans()
							moveconnection = mouse.Move:Connect(function()
								updateTrans()
							end)
							releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
								if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
									updateTrans()
									moveconnection:Disconnect()
									releaseconnection:Disconnect()
								end
							end)
						end)
						Colorpick.MouseButton1Down:Connect(function()
							updateColor()
							moveconnection = mouse.Move:Connect(function()
								updateColor()
							end)
							releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
								if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
									updateColor()
									moveconnection:Disconnect()
									releaseconnection:Disconnect()
								end
							end)
						end)
						Huepick.MouseButton1Down:Connect(function()
							updateHue()
							moveconnection = mouse.Move:Connect(function()
								updateHue()
							end)
							releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
								if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
									updateHue()
									moveconnection:Disconnect()
									releaseconnection:Disconnect()
								end
							end)
						end)
						Button.MouseButton1Down:Connect(function()
							Element.value.Toggle = not Element.value.Toggle;
							update()
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
						end)
						if data.default then
							update()
						end;
						values[tabname][sectorname][tabtext][text] = Element.value;
						function Element:SetValue(value)
							Element.value = value;
							local duplicate = Color3.new(value.Color.R, value.Color.G, value.Color.B)
							ColorH, ColorS, ColorV = duplicate:ToHSV()
							ColorH = math.clamp(ColorH, 0, 1)
							ColorS = math.clamp(ColorS, 0, 1)
							ColorV = math.clamp(ColorV, 0, 1)
							ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
							Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
							ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
							update()
							Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
						end
					elseif type == "Dropdown" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 39)
						Element.value = {
							Dropdown = data.options[1]
						}
						local Dropdown = Instance.new("Frame")
						local Button = Instance.new("TextButton")
						local TextLabel = Instance.new("TextLabel")
						local Drop = Instance.new("ScrollingFrame")
						local Button_2 = Instance.new("TextButton")
						local TextLabel_2 = Instance.new("TextLabel")
						local UIListLayout = Instance.new("UIListLayout")
						local ImageLabel = Instance.new("ImageLabel")
						local TextLabel_3 = Instance.new("TextLabel")
						Dropdown.Name = "Dropdown"
						Dropdown.Parent = tab1;
						Dropdown.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Dropdown.BackgroundTransparency = 1.000;
						Dropdown.Position = UDim2.new(0, 0, 0.255102038, 0)
						Dropdown.Size = UDim2.new(1, 0, 0, 39)
						Button.Name = "Button"
						Button.Parent = Dropdown;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Button.Position = UDim2.new(0, 30, 0, 16)
						Button.Size = UDim2.new(0, 175, 0, 17)
						Button.AutoButtonColor = false;
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						local UIGradient = Instance.new("UIGradient")
						UIGradient.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
							ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
						}
						UIGradient.Rotation = 90;
						UIGradient.Parent = Button;
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
						TextLabel.Position = UDim2.new(0, 5, 0, 0)
						TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = Element.value.Dropdown;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						local abcd = TextLabel;
						Drop.Name = "Drop"
						Drop.Parent = Button;
						Drop.Active = true;
						Drop.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
						Drop.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Drop.Position = UDim2.new(0, 0, 1, 1)
						Drop.Size = UDim2.new(1, 0, 0, 20)
						Drop.Visible = false;
						Drop.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
						Drop.CanvasSize = UDim2.new(1, 1, 1, 1)
						Drop.ScrollBarThickness = 0;
						Drop.MidImage = "http://www.roblox.com/asset/?id=6724808282"
						Drop.TopImage = "http://www.roblox.com/asset/?id=6724808282"
						Drop.AutomaticCanvasSize = "Y"
						Drop.ZIndex = 5;
						Drop.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
						UIListLayout.Parent = Drop;
						UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
						UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
						local num = #data.options;
						if num > 5 then
							Drop.Size = UDim2.new(1, 0, 0, 85)
						else
							Drop.Size = UDim2.new(1, 0, 0, 17 * num)
						end;
						Drop.CanvasSize = UDim2.new(1, 0, 0, 17 * num)
						local first = true;
						for i, v in ipairs(data.options) do
							do
								local Button = Instance.new("TextButton")
								local TextLabel = Instance.new("TextLabel")
								Button.Name = v;
								Button.Parent = Drop;
								Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
								Button.Position = UDim2.new(0, 30, 0, 16)
								Button.Size = UDim2.new(0, 175, 0, 17)
								Button.AutoButtonColor = false;
								Button.Font = Enum.Font.Ubuntu;
								Button.Text = ""
								Button.TextColor3 = Color3.fromRGB(0, 0, 0)
								Button.TextSize = 10.000;
								Button.BorderSizePixel = 0;
								Button.ZIndex = 6;
								TextLabel.Parent = Button;
								TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
								TextLabel.BackgroundTransparency = 1.000;
								TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
								TextLabel.Position = UDim2.new(0, 5, 0, -1)
								TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
								TextLabel.Font = Enum.Font.Ubuntu;
								TextLabel.Text = v;
								TextLabel.TextStrokeTransparency = 0.000;
								TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
								TextLabel.TextSize = 10.000;
								TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
								TextLabel.ZIndex = 6;
								Button.MouseButton1Down:Connect(function()
									Drop.Visible = false;
									Element.value.Dropdown = v;
									abcd.Text = v;
									values[tabname][sectorname][tabtext][text] = Element.value;
									callback(Element.value)
									Drop.CanvasPosition = Vector2.new(0, 0)
								end)
								Button.MouseEnter:Connect(function()
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(124, 81, 149)
									})
								end)
								Button.MouseLeave:Connect(function()
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(255, 255, 255)
									})
								end)
								first = false
							end
						end;
						function Element:SetValue(val)
							Element.value = val;
							abcd.Text = val.Dropdown;
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(val)
						end;
						ImageLabel.Parent = Button;
						ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						ImageLabel.BackgroundTransparency = 1.000;
						ImageLabel.Position = UDim2.new(0, 165, 0, 6)
						ImageLabel.Size = UDim2.new(0, 6, 0, 4)
						ImageLabel.Image = "http://www.roblox.com/asset/?id=6724771531"
						TextLabel_3.Parent = Dropdown;
						TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel_3.BackgroundTransparency = 1.000;
						TextLabel_3.Position = UDim2.new(0, 32, 0, -1)
						TextLabel_3.Size = UDim2.new(0.111913361, 208, 0.382215232, 0)
						TextLabel_3.Font = Enum.Font.Ubuntu;
						TextLabel_3.Text = text;
						TextLabel_3.TextStrokeTransparency = 0.000;
						TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel_3.TextSize = 10.000;
						TextLabel_3.TextXAlignment = Enum.TextXAlignment.Left;
						Button.MouseButton1Down:Connect(function()
							Drop.Visible = not Drop.Visible;
							if not Drop.Visible then
								Drop.CanvasPosition = Vector2.new(0, 0)
							end
						end)
						local indrop = false;
						local ind = false;
						Drop.MouseEnter:Connect(function()
							indrop = true
						end)
						Drop.MouseLeave:Connect(function()
							indrop = false
						end)
						Button.MouseEnter:Connect(function()
							ind = true
						end)
						Button.MouseLeave:Connect(function()
							ind = false
						end)
						game:GetService("UserInputService").InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
								if Drop.Visible == true and not indrop and not ind then
									Drop.Visible = false;
									Drop.CanvasPosition = Vector2.new(0, 0)
								end
							end
						end)
						values[tabname][sectorname][tabtext][text] = Element.value
					elseif type == "Slider" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 25)
						local Slider = Instance.new("Frame")
						local TextLabel = Instance.new("TextLabel")
						local Button = Instance.new("TextButton")
						local Frame = Instance.new("Frame")
						local UIGradient = Instance.new("UIGradient")
						local UIGradient2 = Instance.new("UIGradient")
						local Value = Instance.new("TextLabel")
						Slider.Name = "Slider"
						Slider.Parent = tab1;
						Slider.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Slider.BackgroundTransparency = 1.000;
						Slider.Position = UDim2.new(0, 0, 0.653061211, 0)
						Slider.Size = UDim2.new(1, 0, 0, 25)
						TextLabel.Parent = Slider;
						TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.Position = UDim2.new(0, 32, 0, -2)
						TextLabel.Size = UDim2.new(0, 100, 0, 15)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = text;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						Button.Name = "Button"
						Button.Parent = Slider;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Button.Position = UDim2.new(0, 30, 0, 15)
						Button.Size = UDim2.new(0, 175, 0, 5)
						Button.AutoButtonColor = false;
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						UIGradient2.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
							ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
						}
						UIGradient2.Rotation = 90;
						UIGradient2.Parent = Button;
						Frame.Parent = Button;
						Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Frame.BorderSizePixel = 0;
						Frame.Size = UDim2.new(0.5, 0, 1, 0)
						UIGradient.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(123, 81, 153)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(77, 39, 109))
						}
						UIGradient.Rotation = 90;
						UIGradient.Parent = Frame;
						Value.Name = "Value"
						Value.Parent = Slider;
						Value.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Value.BackgroundTransparency = 1.000;
						Value.Position = UDim2.new(0, 30, 0, 15)
						Value.Size = UDim2.new(0, 175, 0, 5)
						Value.Font = Enum.Font.Ubuntu;
						Value.Text = "50"
						Value.TextStrokeTransparency = 0.000;
						Value.TextColor3 = Color3.fromRGB(255, 255, 255)
						Value.TextSize = 10.000;
						local min, max, default = data.min or 0, data.max or 100, data.default or 0;
						Element.value = {
							Slider = default
						}
						function Element:SetValue(value)
							Element.value = value;
							local a;
							if min > 0 then
								a = ((Element.value.Slider - min)) / (max - min)
							else
								a = (Element.value.Slider - min) / (max - min)
							end;
							Value.Text = Element.value.Slider;
							Frame.Size = UDim2.new(a, 0, 1, 0)
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(value)
						end;
						local a;
						if min > 0 then
							a = ((Element.value.Slider - min)) / (max - min)
						else
							a = (Element.value.Slider - min) / (max - min)
						end;
						Value.Text = Element.value.Slider;
						Frame.Size = UDim2.new(a, 0, 1, 0)
						values[tabname][sectorname][tabtext][text] = Element.value;
						local uis = game:GetService("UserInputService")
						local mouse = game.Players.LocalPlayer:GetMouse()
						local val;
						Button.MouseButton1Down:Connect(function()
							Frame.Size = UDim2.new(0, math.clamp(mouse.X - Frame.AbsolutePosition.X, 0, 175), 0, 5)
							val = math.floor((((tonumber(max) - tonumber(min)) / 175) * Frame.AbsoluteSize.X) + tonumber(min)) or 0;
							Value.Text = val;
							Element.value.Slider = val;
							values[tabname][sectorname][tabtext][text] = Element.value;
							callback(Element.value)
							moveconnection = mouse.Move:Connect(function()
								Frame.Size = UDim2.new(0, math.clamp(mouse.X - Frame.AbsolutePosition.X, 0, 175), 0, 5)
								val = math.floor((((tonumber(max) - tonumber(min)) / 175) * Frame.AbsoluteSize.X) + tonumber(min))
								Value.Text = val;
								Element.value.Slider = val;
								values[tabname][sectorname][tabtext][text] = Element.value;
								callback(Element.value)
							end)
							releaseconnection = uis.InputEnded:Connect(function(Mouse)
								if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
									Frame.Size = UDim2.new(0, math.clamp(mouse.X - Frame.AbsolutePosition.X, 0, 175), 0, 5)
									val = math.floor((((tonumber(max) - tonumber(min)) / 175) * Frame.AbsoluteSize.X) + tonumber(min))
									values[tabname][sectorname][tabtext][text] = Element.value;
									callback(Element.value)
									moveconnection:Disconnect()
									releaseconnection:Disconnect()
								end
							end)
						end)
					elseif type == "Button" then
						tabsize = tabsize + UDim2.new(0, 0, 0, 24)
						local Button = Instance.new("Frame")
						local Button_2 = Instance.new("TextButton")
						local UIGradient = Instance.new("UIGradient")
						local TextLabel = Instance.new("TextLabel")
						Button.Name = "Button"
						Button.Parent = tab1;
						Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button.BackgroundTransparency = 1.000;
						Button.Position = UDim2.new(0, 0, 0.236059487, 0)
						Button.Size = UDim2.new(1, 0, 0, 24)
						Button_2.Name = "Button"
						Button_2.Parent = Button;
						Button_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						Button_2.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Button_2.Position = UDim2.new(0, 30, 0.5, -9)
						Button_2.Size = UDim2.new(0, 175, 0, 18)
						Button_2.AutoButtonColor = false;
						Button_2.Font = Enum.Font.Ubuntu;
						Button_2.Text = ""
						Button_2.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button_2.TextSize = 10.000;
						UIGradient.Color = ColorSequence.new{
							ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
							ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
							ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
						}
						UIGradient.Rotation = 90;
						UIGradient.Parent = Button_2;
						TextLabel.Parent = Button_2;
						TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
						TextLabel.Size = UDim2.new(1, 0, 1, 0)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = text;
						TextLabel.TextStrokeTransparency = 0.000;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						function Element:SetValue()
						end;
						Button_2.MouseButton1Down:Connect(function()
							TextLabel.TextColor3 = Color3.fromRGB(109, 57, 142)
							library:Tween(TextLabel, TweenInfo.new(0.4, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(109, 57, 142)
							})
							callback()
						end)
						Button_2.MouseEnter:Connect(function()
							library:Tween(TextLabel, TweenInfo.new(0.2, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(124, 81, 149)
							})
						end)
						Button_2.MouseLeave:Connect(function()
							library:Tween(TextLabel, TweenInfo.new(0.2, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end)
					end;
					ConfigLoad:Connect(function(cfg)
						local fix = library:ConfigFix(cfg)
						if fix[tabname][sectorname][tabtext][text] ~= nil then
							Element:SetValue(fix[tabname][sectorname][tabtext][text])
						end
					end)
					return Element
				end;
				if firs then
					coroutine.wrap(function()
						game:GetService("RunService").RenderStepped:Wait()
						Section.Size = tabsize
					end)()
					selected = text;
					TextButton.TextColor3 = Color3.fromRGB(255, 255, 255)
					tab1.Visible = true;
					firs = false
				end;
				return tab
			end;
			return MSector
		end;
		function Tab:Sector(text, side)
			local sectorname = text;
			local Sector = {}
			values[tabname][text] = {}
			local Section = Instance.new("Frame")
			local SectionText = Instance.new("TextLabel")
			local Inner = Instance.new("Frame")
			local UIListLayout = Instance.new("UIListLayout")
			local gradient = Instance.new("Frame")
			local UIGradient_2 = Instance.new("UIGradient")
			Section.Name = "Section"
			Section.Parent = TabGui[side]
			Section.BackgroundTransparency = 1.000;
			Section.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
			Section.BorderColor3 = Color3.fromRGB(18, 18, 16)
			Section.BorderSizePixel = 0;
			Section.Position = UDim2.new(0.00358422939, 0, 0, 0)
			Section.Size = UDim2.new(1, 0, 0, 22)
			SectionText.Name = "SectionText"
			SectionText.Parent = Section;
			SectionText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			SectionText.BackgroundTransparency = 1.000;
			SectionText.Position = UDim2.new(0, 7, 0, -4)
			SectionText.Size = UDim2.new(0, 270, 0, 19)
			SectionText.ZIndex = 2;
			SectionText.Font = Enum.Font.Ubuntu;
			SectionText.Text = text;
			SectionText.TextStrokeTransparency = 0.000;
			SectionText.TextColor3 = Color3.fromRGB(255, 255, 255)
			SectionText.TextSize = 12.000;
			SectionText.TextXAlignment = Enum.TextXAlignment.Left;
			gradient.Name = "gradient"
			gradient.Parent = Section;
			gradient.Position = UDim2.new(0.022, 0, 0.035, 0)
			gradient.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			gradient.BorderSizePixel = 0;
			gradient.Position = UDim2.new(0, 0, 0, -3)
			gradient.Size = UDim2.new(0, 280, 0, 2)
			UIGradient_2.Color = ColorSequence.new{
				ColorSequenceKeypoint.new(0.00, Color3.fromRGB(124, 81, 149)),
				ColorSequenceKeypoint.new(0.50, Color3.fromRGB(109, 57, 142)),
				ColorSequenceKeypoint.new(1.00, Color3.fromRGB(79, 48, 112))
			}
			UIGradient_2.Rotation = 90;
			UIGradient_2.Parent = gradient;
			Inner.Name = "Inner"
			Inner.Parent = Section;
			Inner.BackgroundColor3 = Color3.fromRGB(31, 31, 31)
			Inner.BackgroundTransparency = 0.000;
			Inner.BorderColor3 = Color3.fromRGB(18, 18, 16)
			Inner.BorderSizePixel = 2;
			Inner.Position = UDim2.new(0, 1, 0, 1)
			Inner.Size = UDim2.new(1, -2, 1, -2)
			local UIPadding = Instance.new("UIPadding")
			UIPadding.Parent = Inner;
			UIPadding.PaddingTop = UDim.new(0, 10)
			UIListLayout.Parent = Inner;
			UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
			UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
			UIListLayout.Padding = UDim.new(0, 1)
			function Sector:Element(type, text, data, callback)
				local Element = {}
				data = data or {}
				callback = callback or function()
				end;
				values[tabname][sectorname][text] = {}
				if type == "ScrollDrop" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 39)
					Element.value = {
						Scroll = {},
						Dropdown = ""
					}
					for i, v in pairs(data.options) do
						Element.value.Scroll[i] = v[1]
					end;
					local joe = {}
					if data.alphabet then
						local copy = {}
						for i, v in pairs(data.options) do
							table.insert(copy, i)
						end;
						table.sort(copy, function(a, b)
							return a < b
						end)
						joe = copy
					else
						for i, v in pairs(data.options) do
							table.insert(joe, i)
						end
					end;
					local Dropdown = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local TextLabel = Instance.new("TextLabel")
					local Drop = Instance.new("ScrollingFrame")
					local Button_2 = Instance.new("TextButton")
					local TextLabel_2 = Instance.new("TextLabel")
					local UIListLayout = Instance.new("UIListLayout")
					local ImageLabel = Instance.new("ImageLabel")
					local TextLabel_3 = Instance.new("TextLabel")
					Dropdown.Name = "Dropdown"
					Dropdown.Parent = Inner;
					Dropdown.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Dropdown.BackgroundTransparency = 1.000;
					Dropdown.Position = UDim2.new(0, 0, 0, 0)
					Dropdown.Size = UDim2.new(1, 0, 0, 39)
					Button.Name = "Button"
					Button.Parent = Dropdown;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Button.Position = UDim2.new(0, 30, 0, 16)
					Button.Size = UDim2.new(0, 175, 0, 17)
					Button.AutoButtonColor = false;
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					local UIGradient = Instance.new("UIGradient")
					UIGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
					}
					UIGradient.Rotation = 90;
					UIGradient.Parent = Button;
					local TextLabel = Instance.new("TextLabel")
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
					TextLabel.Position = UDim2.new(0, 5, 0, 0)
					TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = "lol"
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local abcd = TextLabel;
					Drop.Name = "Drop"
					Drop.Parent = Button;
					Drop.Active = true;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Drop.Position = UDim2.new(0, 0, 1, 1)
					Drop.Size = UDim2.new(1, 0, 0, 20)
					Drop.Visible = false;
					Drop.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.CanvasSize = UDim2.new(1, 1, 1, 1)
					Drop.ScrollBarThickness = 0;
					Drop.TopImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.MidImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.AutomaticCanvasSize = "Y"
					Drop.ZIndex = 5;
					Drop.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
					local UIGradient2 = Instance.new("UIGradient")
					UIGradient2.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
					}
					UIGradient2.Rotation = 90;
					UIGradient2.Parent = Drop;
					UIListLayout.Parent = Drop;
					UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
					UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
					local amount = data.Amount or 6;
					Section.Size = Section.Size + UDim2.new(0, 0, 0, amount * 16 + 8)
					local num = #joe;
					if num > 5 then
						Drop.Size = UDim2.new(1, 0, 0, 85)
					else
						Drop.Size = UDim2.new(1, 0, 0, 17 * num)
					end;
					local first = true;
					for i, v in ipairs(joe) do
						do
							local joell = v;
							local Scroll = Instance.new("Frame")
							local joe2 = data.options[v]
							local Button = Instance.new("TextButton")
							local TextLabel = Instance.new("TextLabel")
							Button.Name = v;
							Button.Parent = Drop;
							Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Button.Position = UDim2.new(0, 30, 0, 16)
							Button.Size = UDim2.new(0, 175, 0, 17)
							Button.AutoButtonColor = false;
							Button.Font = Enum.Font.Ubuntu;
							Button.Text = ""
							Button.TextColor3 = Color3.fromRGB(0, 0, 0)
							Button.TextSize = 10.000;
							Button.BorderSizePixel = 0;
							Button.ZIndex = 6;
							TextLabel.Parent = Button;
							TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
							TextLabel.BackgroundTransparency = 1.000;
							TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
							TextLabel.Position = UDim2.new(0, 5, 0, -1)
							TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
							TextLabel.Font = Enum.Font.Ubuntu;
							TextLabel.Text = v;
							TextLabel.TextStrokeTransparency = 0.000;
							TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.TextSize = 10.000;
							TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
							TextLabel.ZIndex = 6;
							Button.MouseButton1Down:Connect(function()
								Drop.Visible = false;
								Drop.CanvasPosition = Vector2.new(0, 0)
								abcd.Text = v;
								for i, v in pairs(Scroll.Parent:GetChildren()) do
									if v:IsA("Frame") then
										v.Visible = false
									end
								end;
								Element.value.Dropdown = v;
								Scroll.Visible = true;
								callback(Element.value)
							end)
							Button.MouseEnter:Connect(function()
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end)
							Button.MouseLeave:Connect(function()
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end)
							if first then
								abcd.Text = v;
								Element.value.Dropdown = v
							end;
							local Frame = Instance.new("ScrollingFrame")
							local UIListLayout = Instance.new("UIListLayout")
							Scroll.Name = "Scroll"
							Scroll.Parent = Dropdown;
							Scroll.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
							Scroll.BackgroundTransparency = 1.000;
							Scroll.Position = UDim2.new(0, 0, 0, 0)
							Scroll.Size = UDim2.new(1, 0, 0, amount * 16 + 8)
							Scroll.Visible = first;
							Scroll.Name = v;
							Frame.Name = "Frame"
							Frame.Parent = Scroll;
							Frame.Active = true;
							Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Frame.Position = UDim2.new(0, 30, 0, 40)
							Frame.Size = UDim2.new(0, 175, 0, 16 * amount)
							Frame.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
							Frame.CanvasSize = UDim2.new(0, 0, 0, 0)
							Frame.MidImage = "http://www.roblox.com/asset/?id=6724808282"
							Frame.ScrollBarThickness = 4;
							Frame.TopImage = "http://www.roblox.com/asset/?id=6724808282"
							Frame.AutomaticCanvasSize = "Y"
							Frame.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
							UIListLayout.Parent = Frame;
							UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
							UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
							local joll = true;
							for i, v in ipairs(joe2) do
								local Button = Instance.new("TextButton")
								local TextLabel = Instance.new("TextLabel")
								Button.Name = v;
								Button.Parent = Frame;
								Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
								Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
								Button.BorderSizePixel = 0;
								Button.Position = UDim2.new(0, 30, 0, 16)
								Button.Size = UDim2.new(1, 0, 0, 16)
								Button.AutoButtonColor = false;
								Button.Font = Enum.Font.Ubuntu;
								Button.Text = ""
								Button.TextColor3 = Color3.fromRGB(0, 0, 0)
								Button.TextSize = 10.000;
								TextLabel.Parent = Button;
								TextLabel.BackgroundColor3 = Color3.fromRGB(109, 57, 142)
								TextLabel.BackgroundTransparency = 1.000;
								TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
								TextLabel.Position = UDim2.new(0, 4, 0, -1)
								TextLabel.Size = UDim2.new(1, 1, 1, 1)
								TextLabel.Font = Enum.Font.Ubuntu;
								TextLabel.Text = v;
								TextLabel.TextStrokeTransparency = 0.000;
								TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
								TextLabel.TextSize = 10.000;
								TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
								if joll then
									joll = false;
									TextLabel.TextColor3 = Color3.fromRGB(135, 25, 255)
								end;
								Button.MouseButton1Down:Connect(function()
									for i, v in pairs(Frame:GetChildren()) do
										if v:IsA("TextButton") then
											library:Tween(v.TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
												TextColor3 = Color3.fromRGB(255, 255, 255)
											})
										end
									end;
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(109, 57, 142)
									})
									Element.value.Scroll[joell] = v;
									values[tabname][sectorname][text] = Element.value;
									callback(Element.value)
								end)
								Button.MouseEnter:Connect(function()
									if Element.value.Scroll[joell] ~= v then
										library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(255, 255, 255)
										})
									end
								end)
								Button.MouseLeave:Connect(function()
									if Element.value.Scroll[joell] ~= v then
										library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(255, 255, 255)
										})
									end
								end)
							end;
							first = false
						end
					end;
					ImageLabel.Parent = Button;
					ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					ImageLabel.BackgroundTransparency = 1.000;
					ImageLabel.Position = UDim2.new(0, 165, 0, 6)
					ImageLabel.Size = UDim2.new(0, 6, 0, 4)
					ImageLabel.Image = "http://www.roblox.com/asset/?id=6724771531"
					TextLabel_3.Parent = Dropdown;
					TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel_3.BackgroundTransparency = 1.000;
					TextLabel_3.Position = UDim2.new(0, 32, 0, -1)
					TextLabel_3.Size = UDim2.new(0.111913361, 208, 0.382215232, 0)
					TextLabel_3.Font = Enum.Font.Ubuntu;
					TextLabel_3.Text = text;
					TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel_3.TextSize = 10.000;
					TextLabel_3.TextXAlignment = Enum.TextXAlignment.Left;
					Button.MouseButton1Down:Connect(function()
						Drop.Visible = not Drop.Visible;
						if not Drop.Visible then
							Drop.CanvasPosition = Vector2.new(0, 0)
						end
					end)
					local indrop = false;
					local ind = false;
					Drop.MouseEnter:Connect(function()
						indrop = true
					end)
					Drop.MouseLeave:Connect(function()
						indrop = false
					end)
					Button.MouseEnter:Connect(function()
						ind = true
					end)
					Button.MouseLeave:Connect(function()
						ind = false
					end)
					game:GetService("UserInputService").InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
							if Drop.Visible == true and not indrop and not ind then
								Drop.Visible = false;
								Drop.CanvasPosition = Vector2.new(0, 0)
							end
						end
					end)
					function Element:SetValue(tbl)
						Element.value = tbl;
						abcd.Text = tbl.Dropdown;
						values[tabname][sectorname][text] = Element.value;
						for i, v in pairs(Dropdown:GetChildren()) do
							if v:IsA("Frame") then
								if v.Name == Element.value.Dropdown then
									v.Visible = true
								else
									v.Visible = false
								end;
								for _, bad in pairs(v.Frame:GetChildren()) do
									if bad:IsA("TextButton") then
										bad.TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
										if bad.Name == Element.value.Scroll[v.Name] then
											bad.TextLabel.TextColor3 = Color3.fromRGB(109, 57, 142)
										end
									end
								end
							end
						end
					end;
					if data.default then
						Element:SetValue(data.default)
					end;
					values[tabname][sectorname][text] = Element.value
				elseif type == "Scroll" then
					local amount = data.Amount or 6;
					Section.Size = Section.Size + UDim2.new(0, 0, 0, amount * 16 + 8)
					if data.alphabet then
						table.sort(data.options, function(a, b)
							return a < b
						end)
					end;
					Element.value = {
						Scroll = data.default and data.default.Scroll or data.options[1]
					}
					local Scroll = Instance.new("Frame")
					local Frame = Instance.new("ScrollingFrame")
					local UIListLayout = Instance.new("UIListLayout")
					Scroll.Name = "Scroll"
					Scroll.Parent = Inner;
					Scroll.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Scroll.BackgroundTransparency = 1.000;
					Scroll.Position = UDim2.new(0, 0, 00, 0)
					Scroll.Size = UDim2.new(1, 0, 0, amount * 16 + 8)
					Frame.Name = "Frame"
					Frame.Parent = Scroll;
					Frame.Active = true;
					Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Frame.Position = UDim2.new(0, 30, 0, 0)
					Frame.Size = UDim2.new(0, 175, 0, 16 * amount)
					Frame.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
					Frame.CanvasSize = UDim2.new(0, 0, 0, 0)
					Frame.MidImage = "http://www.roblox.com/asset/?id=6724808282"
					Frame.ScrollBarThickness = 4;
					Frame.TopImage = "http://www.roblox.com/asset/?id=6724808282"
					Frame.AutomaticCanvasSize = "Y"
					Frame.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
					UIListLayout.Parent = Frame;
					UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
					UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
					local first = true;
					for i, v in ipairs(data.options) do
						local Button = Instance.new("TextButton")
						local TextLabel = Instance.new("TextLabel")
						Button.Name = v;
						Button.Parent = Frame;
						Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Button.BorderSizePixel = 0;
						Button.Position = UDim2.new(0, 30, 0, 16)
						Button.Size = UDim2.new(1, 0, 0, 16)
						Button.AutoButtonColor = false;
						Button.Font = Enum.Font.Ubuntu;
						Button.Text = ""
						Button.TextColor3 = Color3.fromRGB(0, 0, 0)
						Button.TextSize = 10.000;
						TextLabel.Parent = Button;
						TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.BackgroundTransparency = 1.000;
						TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
						TextLabel.Position = UDim2.new(0, 4, 0, -1)
						TextLabel.Size = UDim2.new(1, 1, 1, 1)
						TextLabel.Font = Enum.Font.Ubuntu;
						TextLabel.Text = v;
						TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
						TextLabel.TextSize = 10.000;
						TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
						if first then
							first = false;
							TextLabel.TextColor3 = Color3.fromRGB(109, 57, 142)
						end;
						Button.MouseButton1Down:Connect(function()
							for i, v in pairs(Frame:GetChildren()) do
								if v:IsA("TextButton") then
									library:Tween(v.TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(255, 255, 255)
									})
								end
							end;
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(109, 57, 142)
							})
							Element.value.Scroll = v;
							values[tabname][sectorname][text] = Element.value;
							callback(Element.value)
						end)
						Button.MouseEnter:Connect(function()
							if Element.value.Scroll ~= v then
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end
						end)
						Button.MouseLeave:Connect(function()
							if Element.value.Scroll ~= v then
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end
						end)
					end;
					function Element:SetValue(val)
						Element.value = val;
						for i, v in pairs(Frame:GetChildren()) do
							if v:IsA("TextButton") then
								library:Tween(v.TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end
						end;
						library:Tween(Frame[Element.value.Scroll].TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
							TextColor3 = Color3.fromRGB(255, 255, 255)
						})
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end;
					values[tabname][sectorname][text] = Element.value
				elseif type == "Jumbobox" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 39)
					Element.value = {
						Jumbobox = {}
					}
					data.options = data.options or {}
					local Dropdown = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local TextLabel = Instance.new("TextLabel")
					local Drop = Instance.new("ScrollingFrame")
					local Button_2 = Instance.new("TextButton")
					local TextLabel_2 = Instance.new("TextLabel")
					local UIListLayout = Instance.new("UIListLayout")
					local ImageLabel = Instance.new("ImageLabel")
					local TextLabel_3 = Instance.new("TextLabel")
					Dropdown.Name = "Dropdown"
					Dropdown.Parent = Inner;
					Dropdown.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Dropdown.BackgroundTransparency = 1.000;
					Dropdown.Position = UDim2.new(0, 0, 0.255102038, 0)
					Dropdown.Size = UDim2.new(1, 0, 0, 39)
					Button.Name = "Button"
					Button.Parent = Dropdown;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Button.Position = UDim2.new(0, 30, 0, 16)
					Button.Size = UDim2.new(0, 175, 0, 17)
					Button.AutoButtonColor = false;
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					local UIGradient = Instance.new("UIGradient")
					UIGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
					}
					UIGradient.Rotation = 90;
					UIGradient.Parent = Button;
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
					TextLabel.Position = UDim2.new(0, 5, 0, 0)
					TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = "-"
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local abcd = TextLabel;
					Drop.Name = "Drop"
					Drop.Parent = Button;
					Drop.Active = true;
					Drop.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Drop.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Drop.Position = UDim2.new(0, 0, 1, 1)
					Drop.Size = UDim2.new(1, 0, 0, 20)
					Drop.Visible = false;
					Drop.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.CanvasSize = UDim2.new(1, 1, 1, 1)
					Drop.ScrollBarThickness = 0;
					Drop.TopImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.MidImage = "http://www.roblox.com/asset/?id=6724808282"
					for i, v in pairs(data.options) do
						Drop.CanvasSize = Drop.CanvasSize + UDim2.new(0, 0, 0, 17)
					end;
					Drop.ZIndex = 5;
					Drop.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
					UIListLayout.Parent = Drop;
					UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
					UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
					values[tabname][sectorname][text] = Element.value;
					local num = #data.options;
					if num > 5 then
						Drop.Size = UDim2.new(1, 0, 0, 85)
					else
						Drop.Size = UDim2.new(1, 0, 0, 17 * num)
					end;
					local first = true;
					local function updatetext()
						local old = {}
						for i, v in ipairs(data.options) do
							if table.find(Element.value.Jumbobox, v) then
								table.insert(old, v)
							else
							end
						end;
						local str = ""
						if #old == 0 then
							str = "..."
						else
							if #old == 1 then
								str = old[1]
							else
								for i, v in ipairs(old) do
									if i == 1 then
										str = v
									else
										if i > 2 then
											if i < 4 then
												str = str .. ",  ..."
											end
										else
											str = str .. ",  " .. v
										end
									end
								end
							end
						end;
						abcd.Text = str
					end;
					for i, v in ipairs(data.options) do
						do
							local Button = Instance.new("TextButton")
							local TextLabel = Instance.new("TextLabel")
							Button.Name = v;
							Button.Parent = Drop;
							Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Button.Position = UDim2.new(0, 30, 0, 16)
							Button.Size = UDim2.new(0, 175, 0, 17)
							Button.AutoButtonColor = false;
							Button.Font = Enum.Font.Ubuntu;
							Button.Text = ""
							Button.TextColor3 = Color3.fromRGB(0, 0, 0)
							Button.TextSize = 10.000;
							Button.BorderSizePixel = 0;
							Button.ZIndex = 6;
							TextLabel.Parent = Button;
							TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.BackgroundTransparency = 1.000;
							TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
							TextLabel.Position = UDim2.new(0, 5, 0, -1)
							TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
							TextLabel.Font = Enum.Font.Ubuntu;
							TextLabel.Text = v;
							TextLabel.TextStrokeTransparency = 0.000;
							TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.TextSize = 10.000;
							TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
							TextLabel.ZIndex = 6;
							Button.MouseButton1Down:Connect(function()
								if table.find(Element.value.Jumbobox, v) then
									for i, a in pairs(Element.value.Jumbobox) do
										if a == v then
											table.remove(Element.value.Jumbobox, i)
										end
									end;
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(255, 255, 255)
									})
								else
									table.insert(Element.value.Jumbobox, v)
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(255, 255, 255)
									})
								end;
								updatetext()
								values[tabname][sectorname][text] = Element.value;
								callback(Element.value)
							end)
							Button.MouseEnter:Connect(function()
								if not table.find(Element.value.Jumbobox, v) then
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(255, 255, 255)
									})
								end
							end)
							Button.MouseLeave:Connect(function()
								if not table.find(Element.value.Jumbobox, v) then
									library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
										TextColor3 = Color3.fromRGB(255, 255, 255)
									})
								end
							end)
							first = false
						end
					end;
					function Element:SetValue(val)
						Element.value = val;
						for i, v in pairs(Drop:GetChildren()) do
							if v.Name ~= "UIListLayout" then
								if table.find(val.Jumbobox, v.Name) then
									v.TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
								else
									v.TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
								end
							end
						end;
						updatetext()
						values[tabname][sectorname][text] = Element.value;
						callback(val)
					end;
					if data.default then
						Element:SetValue(data.default)
					end;
					ImageLabel.Parent = Button;
					ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					ImageLabel.BackgroundTransparency = 1.000;
					ImageLabel.Position = UDim2.new(0, 165, 0, 6)
					ImageLabel.Size = UDim2.new(0, 6, 0, 4)
					ImageLabel.Image = "http://www.roblox.com/asset/?id=6724771531"
					TextLabel_3.Parent = Dropdown;
					TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel_3.BackgroundTransparency = 1.000;
					TextLabel_3.Position = UDim2.new(0, 32, 0, -1)
					TextLabel_3.Size = UDim2.new(0.111913361, 208, 0.382215232, 0)
					TextLabel_3.Font = Enum.Font.Ubuntu;
					TextLabel_3.Text = text;
					TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel_3.TextSize = 10.000;
					TextLabel_3.TextXAlignment = Enum.TextXAlignment.Left;
					Button.MouseButton1Down:Connect(function()
						Drop.Visible = not Drop.Visible;
						if not Drop.Visible then
							Drop.CanvasPosition = Vector2.new(0, 0)
						end
					end)
					local indrop = false;
					local ind = false;
					Drop.MouseEnter:Connect(function()
						indrop = true
					end)
					Drop.MouseLeave:Connect(function()
						indrop = false
					end)
					Button.MouseEnter:Connect(function()
						ind = true
					end)
					Button.MouseLeave:Connect(function()
						ind = false
					end)
					game:GetService("UserInputService").InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
							if Drop.Visible == true and not indrop and not ind then
								Drop.Visible = false;
								Drop.CanvasPosition = Vector2.new(0, 0)
							end
						end
					end)
				elseif type == "ToggleKeybind" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 16)
					Element.value = {
						Toggle = data.default and data.default.Toggle or false,
						Key,
						Type = "Always",
						Active = true
					}
					local Toggle = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local Color = Instance.new("Frame")
					local TextLabel = Instance.new("TextLabel")
					Toggle.Name = "Toggle"
					Toggle.Parent = Inner;
					Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Toggle.BackgroundTransparency = 1.000;
					Toggle.Size = UDim2.new(1, 0, 0, 15)
					Button.Name = "Button"
					Button.Parent = Toggle;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BackgroundTransparency = 1.000;
					Button.Size = UDim2.new(1, 0, 1, 0)
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					Color.Name = "Color"
					Color.Parent = Button;
					Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Color.Position = UDim2.new(0, 15, 0.5, -5)
					Color.Size = UDim2.new(0, 8, 0, 8)
					local binding = false;
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.Position = UDim2.new(0, 32, 0, -1)
					TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = text;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local function update()
						if Element.value.Toggle then
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(109, 57, 142)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						else
							keybindremove(text)
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end;
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end;
					Button.MouseButton1Down:Connect(function()
						if not binding then
							Element.value.Toggle = not Element.value.Toggle;
							update()
							values[tabname][sectorname][text] = Element.value;
							callback(Element.value)
						end
					end)
					if data.default then
						update()
					end;
					values[tabname][sectorname][text] = Element.value;
					do
						local Keybind = Instance.new("TextButton")
						local Frame = Instance.new("Frame")
						local Always = Instance.new("TextButton")
						local UIListLayout = Instance.new("UIListLayout")
						local Hold = Instance.new("TextButton")
						local Toggle = Instance.new("TextButton")
						Keybind.Name = "Keybind"
						Keybind.Parent = Button;
						Keybind.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Keybind.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Keybind.Position = UDim2.new(0, 270, 0.5, -6)
						Keybind.Text = "none"
						Keybind.BackgroundTransparency = 1.000;
						Keybind.Size = UDim2.new(0, 43, 0, 12)
						Keybind.Size = UDim2.new(0, txt:GetTextSize("none", 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 5, 0, 12)
						Keybind.AutoButtonColor = false;
						Keybind.TextStrokeTransparency = 0.000;
						Keybind.Font = Enum.Font.Ubuntu;
						Keybind.TextColor3 = Color3.fromRGB(255, 255, 255)
						Keybind.TextSize = 10.000;
						Keybind.AnchorPoint = Vector2.new(1, 0)
						Keybind.ZIndex = 3;
						Frame.Parent = Keybind;
						Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Frame.Position = UDim2.new(1, -49, 0, 1)
						Frame.Size = UDim2.new(0, 49, 0, 49)
						Frame.Visible = false;
						Frame.ZIndex = 3;
						Always.Name = "Always"
						Always.Parent = Frame;
						Always.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Always.BackgroundTransparency = 1.000;
						Always.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Always.Position = UDim2.new(-3.03289485, 231, 0.115384616, -6)
						Always.Size = UDim2.new(1, 0, 0, 16)
						Always.AutoButtonColor = false;
						Always.Font = Enum.Font.Ubuntu;
						Always.Text = "Always"
						Always.TextStrokeTransparency = 0.000;
						Always.TextColor3 = Color3.fromRGB(109, 57, 142)
						Always.TextSize = 10.000;
						Always.ZIndex = 3;
						UIListLayout.Parent = Frame;
						UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
						UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
						Hold.Name = "Hold"
						Hold.Parent = Frame;
						Hold.BackgroundColor3 = Color3.fromRGB(146, 46, 46)
						Hold.BackgroundTransparency = 1.000;
						Hold.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Hold.Position = UDim2.new(-3.03289485, 231, 0.115384616, -6)
						Hold.Size = UDim2.new(1, 0, 0, 16)
						Hold.AutoButtonColor = false;
						Hold.Font = Enum.Font.Ubuntu;
						Hold.Text = "Hold"
						Hold.TextStrokeTransparency = 0.000;
						Hold.TextColor3 = Color3.fromRGB(255, 255, 255)
						Hold.TextSize = 10.000;
						Hold.ZIndex = 3;
						Toggle.Name = "Toggle"
						Toggle.Parent = Frame;
						Toggle.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
						Toggle.BackgroundTransparency = 1.000;
						Toggle.BorderColor3 = Color3.fromRGB(18, 18, 16)
						Toggle.Position = UDim2.new(-3.03289485, 231, 0.115384616, -6)
						Toggle.Size = UDim2.new(1, 0, 0, 16)
						Toggle.AutoButtonColor = false;
						Toggle.Font = Enum.Font.Ubuntu;
						Toggle.Text = "Toggle"
						Toggle.TextStrokeTransparency = 0.000;
						Toggle.TextColor3 = Color3.fromRGB(255, 255, 255)
						Toggle.TextSize = 10.000;
						Toggle.ZIndex = 3;
						for _, button in pairs(Frame:GetChildren()) do
							if button:IsA("TextButton") then
								button.MouseButton1Down:Connect(function()
									Element.value.Type = button.Text;
									Frame.Visible = false;
									if Element.value.Active ~= (Element.value.Type == "Always" and true or false) then
										Element.value.Active = Element.value.Type == "Always" and true or false;
										callback(Element.value)
									end;
									if button.Text == "Always" then
										keybindremove(text)
									end;
									for _, button in pairs(Frame:GetChildren()) do
										if button:IsA("TextButton") and button.Text ~= Element.value.Type then
											button.Font = Enum.Font.Ubuntu;
											library:Tween(button, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
												TextColor3 = Color3.fromRGB(255, 255, 255)
											})
										end
									end;
									button.Font = Enum.Font.Ubuntu;
									button.TextColor3 = Color3.fromRGB(109, 57, 142)
									values[tabname][sectorname][text] = Element.value
								end)
								button.MouseEnter:Connect(function()
									if Element.value.Type ~= button.Text then
										library:Tween(button, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(155, 155, 155)
										})
									end
								end)
								button.MouseLeave:Connect(function()
									if Element.value.Type ~= button.Text then
										library:Tween(button, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
											TextColor3 = Color3.fromRGB(155, 155, 155)
										})
									end
								end)
							end
						end;
						Keybind.MouseButton1Down:Connect(function()
							if not binding then
								wait()
								binding = true;
								Keybind.Text = "-"
								Keybind.Size = UDim2.new(0, txt:GetTextSize("-", 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 4, 0, 12)
							end
						end)
						Keybind.MouseButton2Down:Connect(function()
							if not binding then
								Frame.Visible = not Frame.Visible
							end
						end)
						local Player = game.Players.LocalPlayer;
						local Mouse = Player:GetMouse()
						local InFrame = false;
						Frame.MouseEnter:Connect(function()
							InFrame = true
						end)
						Frame.MouseLeave:Connect(function()
							InFrame = false
						end)
						local InFrame2 = false;
						Keybind.MouseEnter:Connect(function()
							InFrame2 = true
						end)
						Keybind.MouseLeave:Connect(function()
							InFrame2 = false
						end)
						game:GetService("UserInputService").InputBegan:Connect(function(input)
							if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 and not binding then
								if Frame.Visible == true and not InFrame and not InFrame2 then
									Frame.Visible = false
								end
							end;
							if binding then
								binding = false;
								Keybind.Text = input.KeyCode.Name ~= "Unknown" and input.KeyCode.Name:upper() or input.UserInputType.Name:upper()
								Keybind.Size = UDim2.new(0, txt:GetTextSize(Keybind.Text, 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 5, 0, 12)
								Element.value.Key = input.KeyCode.Name ~= "Unknown" and input.KeyCode.Name or input.UserInputType.Name;
								if input.KeyCode.Name == "Backspace" then
									Keybind.Text = "none"
									Keybind.Size = UDim2.new(0, txt:GetTextSize(Keybind.Text, 14, Enum.Font.Ubuntu, Vector2.new(700, 12)).X + 4, 0, 12)
									Element.value.Key = nil;
									Element.value.Active = true
								end;
								callback(Element.value)
							else
								if Element.value.Key ~= nil then
									if string.find(Element.value.Key, "Mouse") then
										if input.UserInputType == Enum.UserInputType[Element.value.Key] then
											if Element.value.Type == "Hold" then
												Element.value.Active = true;
												callback(Element.value)
												if Element.value.Active and Element.value.Toggle then
													keybindhold(text)
												else
													keybindremove(text)
												end
											elseif Element.value.Type == "Toggle" then
												Element.value.Active = not Element.value.Active;
												callback(Element.value)
												if Element.value.Active and Element.value.Toggle then
													keybindadd(text)
												else
													keybindremove(text)
												end
											end
										end
									else
										if input.KeyCode == Enum.KeyCode[Element.value.Key] then
											if Element.value.Type == "Hold" then
												Element.value.Active = true;
												callback(Element.value)
												if Element.value.Active and Element.value.Toggle then
													keybindhold(text)
												else
													keybindremove(text)
												end
											elseif Element.value.Type == "Toggle" then
												Element.value.Active = not Element.value.Active;
												callback(Element.value)
												if Element.value.Active and Element.value.Toggle then
													keybindadd(text)
												else
													keybindremove(text)
												end
											end
										end
									end
								else
									Element.value.Active = true
								end
							end;
							values[tabname][sectorname][text] = Element.value
						end)
						game:GetService("UserInputService").InputEnded:Connect(function(input)
							if Element.value.Key ~= nil then
								if string.find(Element.value.Key, "Mouse") then
									if input.UserInputType == Enum.UserInputType[Element.value.Key] then
										if Element.value.Type == "Hold" then
											Element.value.Active = false;
											callback(Element.value)
											if Element.value.Active then
												keybindhold(text)
											else
												keybindremove(text)
											end
										end
									end
								else
									if input.KeyCode == Enum.KeyCode[Element.value.Key] then
										if Element.value.Type == "Hold" then
											Element.value.Active = false;
											callback(Element.value)
											if Element.value.Active then
												keybindhold(text)
											else
												keybindremove(text)
											end
										end
									end
								end
							end;
							values[tabname][sectorname][text] = Element.value
						end)
					end;
					function Element:SetValue(value)
						Element.value = value;
						update()
					end
				elseif type == "Toggle" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 16)
					Element.value = {
						Toggle = data.default and data.default.Toggle or false
					}
					local Toggle = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local Color = Instance.new("Frame")
					local TextLabel = Instance.new("TextLabel")
					Toggle.Name = "Toggle"
					Toggle.Parent = Inner;
					Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Toggle.BackgroundTransparency = 1.000;
					Toggle.Size = UDim2.new(1, 0, 0, 15)
					Button.Name = "Button"
					Button.Parent = Toggle;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BackgroundTransparency = 1.000;
					Button.Size = UDim2.new(1, 0, 1, 0)
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					Color.Name = "Color"
					Color.Parent = Button;
					Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Color.Position = UDim2.new(0, 15, 0.5, -5)
					Color.Size = UDim2.new(0, 8, 0, 8)
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.Position = UDim2.new(0, 32, 0, -1)
					TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = text;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local function update()
						if Element.value.Toggle then
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(109, 57, 142)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						else
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end;
						values[tabname][sectorname][text] = Element.value
					end;
					Button.MouseButton1Down:Connect(function()
						Element.value.Toggle = not Element.value.Toggle;
						update()
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end)
					if data.default then
						update()
					end;
					values[tabname][sectorname][text] = Element.value;
					function Element:SetValue(value)
						Element.value = value;
						values[tabname][sectorname][text] = Element.value;
						update()
						callback(Element.value)
					end
				elseif type == "ToggleColor" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 16)
					Element.value = {
						Toggle = data.default and data.default.Toggle or false,
						Color = data.default and data.default.Color or Color3.fromRGB(255, 255, 255)
					}
					local Toggle = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local Color = Instance.new("Frame")
					local TextLabel = Instance.new("TextLabel")
					Toggle.Name = "Toggle"
					Toggle.Parent = Inner;
					Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Toggle.BackgroundTransparency = 1.000;
					Toggle.Size = UDim2.new(1, 0, 0, 15)
					Button.Name = "Button"
					Button.Parent = Toggle;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BackgroundTransparency = 1.000;
					Button.Size = UDim2.new(1, 0, 1, 0)
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					Color.Name = "Color"
					Color.Parent = Button;
					Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Color.Position = UDim2.new(0, 15, 0.5, -5)
					Color.Size = UDim2.new(0, 8, 0, 8)
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.Position = UDim2.new(0, 32, 0, -1)
					TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = text;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local function update()
						if Element.value.Toggle then
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(109, 57, 142)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						else
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end;
						values[tabname][sectorname][text] = Element.value
					end;
					local ColorH, ColorS, ColorV;
					local ColorP = Instance.new("TextButton")
					local Frame = Instance.new("Frame")
					local Colorpick = Instance.new("ImageButton")
					local ColorDrag = Instance.new("Frame")
					local Huepick = Instance.new("ImageButton")
					local Huedrag = Instance.new("Frame")
					ColorP.Name = "ColorP"
					ColorP.Parent = Button;
					ColorP.AnchorPoint = Vector2.new(1, 0)
					ColorP.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
					ColorP.BorderColor3 = Color3.fromRGB(18, 18, 16)
					ColorP.Position = UDim2.new(0, 270, 0.5, -4)
					ColorP.Size = UDim2.new(0, 18, 0, 8)
					ColorP.AutoButtonColor = false;
					ColorP.Font = Enum.Font.Ubuntu;
					ColorP.Text = ""
					ColorP.TextColor3 = Color3.fromRGB(255, 255, 255)
					ColorP.TextSize = 10.000;
					Frame.Parent = ColorP;
					Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Frame.Position = UDim2.new(-0.666666687, -170, 1.375, 0)
					Frame.Size = UDim2.new(0, 200, 0, 170)
					Frame.Visible = false;
					Frame.ZIndex = 3;
					Colorpick.Name = "Colorpick"
					Colorpick.Parent = Frame;
					Colorpick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Colorpick.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Colorpick.ClipsDescendants = false;
					Colorpick.Position = UDim2.new(0, 40, 0, 10)
					Colorpick.Size = UDim2.new(0, 150, 0, 150)
					Colorpick.AutoButtonColor = false;
					Colorpick.Image = "rbxassetid://4155801252"
					Colorpick.ImageColor3 = Color3.fromRGB(255, 0, 0)
					Colorpick.ZIndex = 3;
					ColorDrag.Name = "ColorDrag"
					ColorDrag.Parent = Colorpick;
					ColorDrag.AnchorPoint = Vector2.new(0.5, 0.5)
					ColorDrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					ColorDrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
					ColorDrag.Size = UDim2.new(0, 4, 0, 4)
					ColorDrag.ZIndex = 3;
					Huepick.Name = "Huepick"
					Huepick.Parent = Frame;
					Huepick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Huepick.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Huepick.ClipsDescendants = false;
					Huepick.Position = UDim2.new(0, 10, 0, 10)
					Huepick.Size = UDim2.new(0, 20, 0, 150)
					Huepick.AutoButtonColor = false;
					Huepick.Image = "rbxassetid://3641079629"
					Huepick.ImageColor3 = Color3.fromRGB(255, 0, 0)
					Huepick.ImageTransparency = 1;
					Huepick.BackgroundTransparency = 0;
					Huepick.ZIndex = 3;
					local HueFrameGradient = Instance.new("UIGradient")
					HueFrameGradient.Rotation = 90;
					HueFrameGradient.Name = "HueFrameGradient"
					HueFrameGradient.Parent = Huepick;
					HueFrameGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 0, 0)),
						ColorSequenceKeypoint.new(0.17, Color3.fromRGB(255, 0, 255)),
						ColorSequenceKeypoint.new(0.33, Color3.fromRGB(0, 0, 255)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(0, 255, 255)),
						ColorSequenceKeypoint.new(0.67, Color3.fromRGB(0, 255, 0)),
						ColorSequenceKeypoint.new(0.83, Color3.fromRGB(255, 255, 0)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 0, 0))
					}
					Huedrag.Name = "Huedrag"
					Huedrag.Parent = Huepick;
					Huedrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Huedrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Huedrag.Size = UDim2.new(1, 0, 0, 2)
					Huedrag.ZIndex = 3;
					ColorP.MouseButton1Down:Connect(function()
						Frame.Visible = not Frame.Visible
					end)
					local abc = false;
					local inCP = false;
					ColorP.MouseEnter:Connect(function()
						abc = true
					end)
					ColorP.MouseLeave:Connect(function()
						abc = false
					end)
					Frame.MouseEnter:Connect(function()
						inCP = true
					end)
					Frame.MouseLeave:Connect(function()
						inCP = false
					end)
					ColorH = (math.clamp(Huedrag.AbsolutePosition.Y - Huepick.AbsolutePosition.Y, 0, Huepick.AbsoluteSize.Y) / Huepick.AbsoluteSize.Y)
					ColorS = 1 - (math.clamp(ColorDrag.AbsolutePosition.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
					ColorV = 1 - (math.clamp(ColorDrag.AbsolutePosition.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
					if data.default and data.default.Color ~= nil then
						ColorH, ColorS, ColorV = data.default.Color:ToHSV()
						ColorH = math.clamp(ColorH, 0, 1)
						ColorS = math.clamp(ColorS, 0, 1)
						ColorV = math.clamp(ColorV, 0, 1)
						ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
						values[tabname][sectorname][text] = data.default.Color
					end;
					local mouse = LocalPlayer:GetMouse()
					game:GetService("UserInputService").InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
							if not dragging and not abc and not inCP then
								Frame.Visible = false
							end
						end
					end)
					local function updateColor()
						local ColorX = (math.clamp(mouse.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
						local ColorY = (math.clamp(mouse.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
						ColorDrag.Position = UDim2.new(ColorX, 0, ColorY, 0)
						ColorS = 1 - ColorX;
						ColorV = 1 - ColorY;
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						values[tabname][sectorname][text] = Element.value;
						Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
						callback(Element.value)
					end;
					local function updateHue()
						local y = math.clamp(mouse.Y - Huepick.AbsolutePosition.Y, 0, 148)
						Huedrag.Position = UDim2.new(0, 0, 0, y)
						hue = y / 148;
						ColorH = 1 - hue;
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						values[tabname][sectorname][text] = Element.value;
						Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
						callback(Element.value)
					end;
					Colorpick.MouseButton1Down:Connect(function()
						updateColor()
						moveconnection = mouse.Move:Connect(function()
							updateColor()
						end)
						releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
							if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
								updateColor()
								moveconnection:Disconnect()
								releaseconnection:Disconnect()
							end
						end)
					end)
					Huepick.MouseButton1Down:Connect(function()
						updateHue()
						moveconnection = mouse.Move:Connect(function()
							updateHue()
						end)
						releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
							if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
								updateHue()
								moveconnection:Disconnect()
								releaseconnection:Disconnect()
							end
						end)
					end)
					Button.MouseButton1Down:Connect(function()
						Element.value.Toggle = not Element.value.Toggle;
						update()
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end)
					if data.default then
						update()
					end;
					values[tabname][sectorname][text] = Element.value;
					function Element:SetValue(value)
						Element.value = value;
						local duplicate = Color3.new(value.Color.R, value.Color.G, value.Color.B)
						ColorH, ColorS, ColorV = duplicate:ToHSV()
						ColorH = math.clamp(ColorH, 0, 1)
						ColorS = math.clamp(ColorS, 0, 1)
						ColorV = math.clamp(ColorV, 0, 1)
						ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						update()
						Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
						callback(value)
					end
				elseif type == "ToggleTrans" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 16)
					Element.value = {
						Toggle = data.default and data.default.Toggle or false,
						Color = data.default and data.default.Color or Color3.fromRGB(255, 255, 255),
						Transparency = data.default and data.default.Transparency or 0
					}
					local Toggle = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local Color = Instance.new("Frame")
					local TextLabel = Instance.new("TextLabel")
					Toggle.Name = "Toggle"
					Toggle.Parent = Inner;
					Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Toggle.BackgroundTransparency = 1.000;
					Toggle.Size = UDim2.new(1, 0, 0, 15)
					Button.Name = "Button"
					Button.Parent = Toggle;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BackgroundTransparency = 1.000;
					Button.Size = UDim2.new(1, 0, 1, 0)
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					Color.Name = "Color"
					Color.Parent = Button;
					Color.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Color.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Color.Position = UDim2.new(0, 15, 0.5, -5)
					Color.Size = UDim2.new(0, 8, 0, 8)
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.Position = UDim2.new(0, 32, 0, -1)
					TextLabel.Size = UDim2.new(0.111913361, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = text;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local function update()
						if Element.value.Toggle then
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(109, 57, 142)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						else
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							})
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BorderColor3 = Color3.fromRGB(18, 18, 16)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end;
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end;
					local ColorH, ColorS, ColorV;
					local ColorP = Instance.new("TextButton")
					local Frame = Instance.new("Frame")
					local Colorpick = Instance.new("ImageButton")
					local ColorDrag = Instance.new("Frame")
					local Huepick = Instance.new("ImageButton")
					local Huedrag = Instance.new("Frame")
					ColorP.Name = "ColorP"
					ColorP.Parent = Button;
					ColorP.AnchorPoint = Vector2.new(1, 0)
					ColorP.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
					ColorP.BorderColor3 = Color3.fromRGB(18, 18, 16)
					ColorP.Position = UDim2.new(0, 270, 0.5, -4)
					ColorP.Size = UDim2.new(0, 18, 0, 8)
					ColorP.AutoButtonColor = false;
					ColorP.Font = Enum.Font.Ubuntu;
					ColorP.Text = ""
					ColorP.TextColor3 = Color3.fromRGB(255, 255, 255)
					ColorP.TextSize = 10.000;
					Frame.Parent = ColorP;
					Frame.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Frame.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Frame.Position = UDim2.new(-0.666666687, -170, 1.375, 0)
					Frame.Size = UDim2.new(0, 200, 0, 190)
					Frame.Visible = false;
					Frame.ZIndex = 3;
					Colorpick.Name = "Colorpick"
					Colorpick.Parent = Frame;
					Colorpick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Colorpick.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Colorpick.ClipsDescendants = false;
					Colorpick.Position = UDim2.new(0, 40, 0, 10)
					Colorpick.Size = UDim2.new(0, 150, 0, 150)
					Colorpick.AutoButtonColor = false;
					Colorpick.Image = "rbxassetid://4155801252"
					Colorpick.ImageColor3 = Color3.fromRGB(255, 0, 0)
					Colorpick.ZIndex = 3;
					ColorDrag.Name = "ColorDrag"
					ColorDrag.Parent = Colorpick;
					ColorDrag.AnchorPoint = Vector2.new(0.5, 0.5)
					ColorDrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					ColorDrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
					ColorDrag.Size = UDim2.new(0, 4, 0, 4)
					ColorDrag.ZIndex = 3;
					Huepick.Name = "Huepick"
					Huepick.Parent = Frame;
					Huepick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Huepick.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Huepick.ClipsDescendants = true;
					Huepick.Position = UDim2.new(0, 10, 0, 10)
					Huepick.Size = UDim2.new(0, 20, 0, 150)
					Huepick.AutoButtonColor = false;
					Huepick.Image = "rbxassetid://3641079629"
					Huepick.ImageColor3 = Color3.fromRGB(255, 0, 0)
					Huepick.ImageTransparency = 1;
					Huepick.BackgroundTransparency = 0;
					Huepick.ZIndex = 3;
					local HueFrameGradient = Instance.new("UIGradient")
					HueFrameGradient.Rotation = 90;
					HueFrameGradient.Name = "HueFrameGradient"
					HueFrameGradient.Parent = Huepick;
					HueFrameGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 0, 0)),
						ColorSequenceKeypoint.new(0.17, Color3.fromRGB(255, 0, 255)),
						ColorSequenceKeypoint.new(0.33, Color3.fromRGB(0, 0, 255)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(0, 255, 255)),
						ColorSequenceKeypoint.new(0.67, Color3.fromRGB(0, 255, 0)),
						ColorSequenceKeypoint.new(0.83, Color3.fromRGB(255, 255, 0)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 0, 0))
					}
					Huedrag.Name = "Huedrag"
					Huedrag.Parent = Huepick;
					Huedrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Huedrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Huedrag.Size = UDim2.new(1, 0, 0, 2)
					Huedrag.ZIndex = 3;
					local Transpick = Instance.new("ImageButton")
					local Transcolor = Instance.new("ImageLabel")
					local Transdrag = Instance.new("Frame")
					Transpick.Name = "Transpick"
					Transpick.Parent = Frame;
					Transpick.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Transpick.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Transpick.Position = UDim2.new(0, 10, 0, 167)
					Transpick.Size = UDim2.new(0, 180, 0, 15)
					Transpick.AutoButtonColor = false;
					Transpick.Image = "rbxassetid://3887014957"
					Transpick.ScaleType = Enum.ScaleType.Tile;
					Transpick.TileSize = UDim2.new(0, 10, 0, 10)
					Transpick.ZIndex = 3;
					Transcolor.Name = "Transcolor"
					Transcolor.Parent = Transpick;
					Transcolor.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Transcolor.BackgroundTransparency = 1.000;
					Transcolor.Size = UDim2.new(1, 0, 1, 0)
					Transcolor.Image = "rbxassetid://3887017050"
					Transcolor.ImageColor3 = Color3.fromRGB(255, 0, 4)
					Transcolor.ZIndex = 3;
					Transdrag.Name = "Transdrag"
					Transdrag.Parent = Transcolor;
					Transdrag.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Transdrag.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Transdrag.Position = UDim2.new(0, -1, 0, 0)
					Transdrag.Size = UDim2.new(0, 2, 1, 0)
					Transdrag.ZIndex = 3;
					ColorP.MouseButton1Down:Connect(function()
						Frame.Visible = not Frame.Visible
					end)
					local abc = false;
					local inCP = false;
					ColorP.MouseEnter:Connect(function()
						abc = true
					end)
					ColorP.MouseLeave:Connect(function()
						abc = false
					end)
					Frame.MouseEnter:Connect(function()
						inCP = true
					end)
					Frame.MouseLeave:Connect(function()
						inCP = false
					end)
					ColorH = (math.clamp(Huedrag.AbsolutePosition.Y - Huepick.AbsolutePosition.Y, 0, Huepick.AbsoluteSize.Y) / Huepick.AbsoluteSize.Y)
					ColorS = 1 - (math.clamp(ColorDrag.AbsolutePosition.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
					ColorV = 1 - (math.clamp(ColorDrag.AbsolutePosition.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
					if data.default and data.default.Color ~= nil then
						ColorH, ColorS, ColorV = data.default.Color:ToHSV()
						ColorH = math.clamp(ColorH, 0, 1)
						ColorS = math.clamp(ColorS, 0, 1)
						ColorV = math.clamp(ColorV, 0, 1)
						ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						Transcolor.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
					end;
					if data.default and data.default.Transparency ~= nil then
						Transdrag.Position = UDim2.new(data.default.Transparency, -1, 0, 0)
					end;
					local mouse = LocalPlayer:GetMouse()
					game:GetService("UserInputService").InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
							if not dragging and not abc and not inCP then
								Frame.Visible = false
							end
						end
					end)
					local function updateColor()
						local ColorX = (math.clamp(mouse.X - Colorpick.AbsolutePosition.X, 0, Colorpick.AbsoluteSize.X) / Colorpick.AbsoluteSize.X)
						local ColorY = (math.clamp(mouse.Y - Colorpick.AbsolutePosition.Y, 0, Colorpick.AbsoluteSize.Y) / Colorpick.AbsoluteSize.Y)
						ColorDrag.Position = UDim2.new(ColorX, 0, ColorY, 0)
						ColorS = 1 - ColorX;
						ColorV = 1 - ColorY;
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						Transcolor.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						values[tabname][sectorname][text] = Element.value;
						Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
						callback(Element.value)
					end;
					local function updateHue()
						local y = math.clamp(mouse.Y - Huepick.AbsolutePosition.Y, 0, 148)
						Huedrag.Position = UDim2.new(0, 0, 0, y)
						hue = y / 148;
						ColorH = 1 - hue;
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						Transcolor.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						values[tabname][sectorname][text] = Element.value;
						Element.value.Color = Color3.fromHSV(ColorH, ColorS, ColorV)
						callback(Element.value)
					end;
					local function updateTrans()
						local x = math.clamp(mouse.X - Transpick.AbsolutePosition.X, 0, 178)
						Transdrag.Position = UDim2.new(0, x, 0, 0)
						Element.value.Transparency = (x / 178)
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end;
					Transpick.MouseButton1Down:Connect(function()
						updateTrans()
						moveconnection = mouse.Move:Connect(function()
							updateTrans()
						end)
						releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
							if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
								updateTrans()
								moveconnection:Disconnect()
								releaseconnection:Disconnect()
							end
						end)
					end)
					Colorpick.MouseButton1Down:Connect(function()
						updateColor()
						moveconnection = mouse.Move:Connect(function()
							updateColor()
						end)
						releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
							if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
								updateColor()
								moveconnection:Disconnect()
								releaseconnection:Disconnect()
							end
						end)
					end)
					Huepick.MouseButton1Down:Connect(function()
						updateHue()
						moveconnection = mouse.Move:Connect(function()
							updateHue()
						end)
						releaseconnection = game:GetService("UserInputService").InputEnded:Connect(function(Mouse)
							if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
								updateHue()
								moveconnection:Disconnect()
								releaseconnection:Disconnect()
							end
						end)
					end)
					Button.MouseButton1Down:Connect(function()
						Element.value.Toggle = not Element.value.Toggle;
						update()
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end)
					if data.default then
						if Element.value.Toggle then
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(109, 57, 142)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						else
							tween = library:Tween(Color, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							})
							library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
								TextColor3 = Color3.fromRGB(255, 255, 255)
							})
						end;
						values[tabname][sectorname][text] = Element.value
					end;
					values[tabname][sectorname][text] = Element.value;
					function Element:SetValue(value)
						Element.value = value;
						local duplicate = Color3.new(value.Color.R, value.Color.G, value.Color.B)
						ColorH, ColorS, ColorV = duplicate:ToHSV()
						ColorH = math.clamp(ColorH, 0, 1)
						ColorS = math.clamp(ColorS, 0, 1)
						ColorV = math.clamp(ColorV, 0, 1)
						ColorDrag.Position = UDim2.new(1 - ColorS, 0, 1 - ColorV, 0)
						Colorpick.ImageColor3 = Color3.fromHSV(ColorH, 1, 1)
						ColorP.BackgroundColor3 = Color3.fromHSV(ColorH, ColorS, ColorV)
						update()
						Huedrag.Position = UDim2.new(0, 0, 1 - ColorH, -1)
					end
				elseif type == "TextBox" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 30)
					Element.value = {
						Text = data.default and data.default.text or ""
					}
					local Box = Instance.new("Frame")
					local TextBox = Instance.new("TextBox")
					Box.Name = "Box"
					Box.Parent = Inner;
					Box.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Box.BackgroundTransparency = 1.000;
					Box.Position = UDim2.new(0, 0, 0.542059898, 0)
					Box.Size = UDim2.new(1, 0, 0, 30)
					TextBox.Parent = Box;
					TextBox.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
					TextBox.BorderColor3 = Color3.fromRGB(18, 18, 16)
					TextBox.Position = UDim2.new(0.108303241, 0, 0.224465579, 0)
					TextBox.Size = UDim2.new(0, 175, 0, 20)
					TextBox.Font = Enum.Font.Ubuntu;
					TextBox.PlaceholderText = data.placeholder;
					TextBox.Text = Element.value.Text;
					TextBox.TextTruncate = 1;
					TextBox.MultiLine = true;
					TextBox.ClearTextOnFocus = false;
					TextBox.TextStrokeTransparency = 0.000;
					TextBox.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextBox.TextSize = 10.000;
					values[tabname][sectorname][text] = Element.value;
					TextBox:GetPropertyChangedSignal("Text"):Connect(function()
						Element.value.Text = TextBox.Text;
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
					end)
					function Element:SetValue(value)
						Element.value = value;
						values[tabname][sectorname][text] = Element.value;
						TextBox.Text = Element.value.Text
					end
				elseif type == "Dropdown" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 39)
					Element.value = {
						Dropdown = data.options[1]
					}
					local Dropdown = Instance.new("Frame")
					local Button = Instance.new("TextButton")
					local TextLabel = Instance.new("TextLabel")
					local Drop = Instance.new("ScrollingFrame")
					local Button_2 = Instance.new("TextButton")
					local TextLabel_2 = Instance.new("TextLabel")
					local UIListLayout = Instance.new("UIListLayout")
					local ImageLabel = Instance.new("ImageLabel")
					local TextLabel_3 = Instance.new("TextLabel")
					Dropdown.Name = "Dropdown"
					Dropdown.Parent = Inner;
					Dropdown.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Dropdown.BackgroundTransparency = 1.000;
					Dropdown.Position = UDim2.new(0, 0, 0.255102038, 0)
					Dropdown.Size = UDim2.new(1, 0, 0, 39)
					Button.Name = "Button"
					Button.Parent = Dropdown;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Button.Position = UDim2.new(0, 30, 0, 16)
					Button.Size = UDim2.new(0, 175, 0, 17)
					Button.AutoButtonColor = false;
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					local UIGradient = Instance.new("UIGradient")
					UIGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
					}
					UIGradient.Rotation = 90;
					UIGradient.Parent = Button;
					TextLabel.Parent = Button;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
					TextLabel.Position = UDim2.new(0, 5, 0, 0)
					TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = Element.value.Dropdown;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					local abcd = TextLabel;
					Drop.Name = "Drop"
					Drop.Parent = Button;
					Drop.Active = true;
					Drop.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
					Drop.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Drop.Position = UDim2.new(0, 0, 1, 1)
					Drop.Size = UDim2.new(1, 0, 0, 20)
					Drop.Visible = false;
					Drop.BottomImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.CanvasSize = UDim2.new(1, 1, 1, 1)
					Drop.ScrollBarThickness = 4;
					Drop.TopImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.MidImage = "http://www.roblox.com/asset/?id=6724808282"
					Drop.AutomaticCanvasSize = "Y"
					Drop.ZIndex = 5;
					Drop.ScrollBarImageColor3 = Color3.fromRGB(109, 57, 142)
					UIListLayout.Parent = Drop;
					UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center;
					UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder;
					local num = #data.options;
					if num > 5 then
						Drop.Size = UDim2.new(1, 0, 0, 85)
					else
						Drop.Size = UDim2.new(1, 0, 0, 17 * num)
					end;
					local first = true;
					for i, v in ipairs(data.options) do
						do
							local Button = Instance.new("TextButton")
							local TextLabel = Instance.new("TextLabel")
							Button.Name = v;
							Button.Parent = Drop;
							Button.BackgroundColor3 = Color3.fromRGB(46, 46, 46)
							Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
							Button.Position = UDim2.new(0, 30, 0, 16)
							Button.Size = UDim2.new(0, 175, 0, 17)
							Button.AutoButtonColor = false;
							Button.Font = Enum.Font.Ubuntu;
							Button.Text = ""
							Button.TextColor3 = Color3.fromRGB(0, 0, 0)
							Button.TextSize = 10.000;
							Button.BorderSizePixel = 0;
							Button.ZIndex = 6;
							TextLabel.Parent = Button;
							TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.BackgroundTransparency = 1.000;
							TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
							TextLabel.Position = UDim2.new(0, 5, 0, -1)
							TextLabel.Size = UDim2.new(-0.21714285, 208, 1, 0)
							TextLabel.Font = Enum.Font.Ubuntu;
							TextLabel.Text = v;
							TextLabel.TextStrokeTransparency = 0.000;
							TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.TextSize = 10.000;
							TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
							TextLabel.ZIndex = 6;
							Button.MouseButton1Down:Connect(function()
								Drop.Visible = false;
								Element.value.Dropdown = v;
								abcd.Text = v;
								values[tabname][sectorname][text] = Element.value;
								callback(Element.value)
								Drop.CanvasPosition = Vector2.new(0, 0)
							end)
							Button.MouseEnter:Connect(function()
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(109, 57, 142)
								})
							end)
							Button.MouseLeave:Connect(function()
								library:Tween(TextLabel, TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
									TextColor3 = Color3.fromRGB(255, 255, 255)
								})
							end)
							first = false
						end
					end;
					function Element:SetValue(val)
						Element.value = val;
						abcd.Text = val.Dropdown;
						values[tabname][sectorname][text] = Element.value;
						callback(val)
					end;
					ImageLabel.Parent = Button;
					ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					ImageLabel.BackgroundTransparency = 1.000;
					ImageLabel.Position = UDim2.new(0, 165, 0, 6)
					ImageLabel.Size = UDim2.new(0, 6, 0, 4)
					ImageLabel.Image = "http://www.roblox.com/asset/?id=6724771531"
					TextLabel_3.Parent = Dropdown;
					TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel_3.BackgroundTransparency = 1.000;
					TextLabel_3.Position = UDim2.new(0, 32, 0, -1)
					TextLabel_3.Size = UDim2.new(0.111913361, 208, 0.382215232, 0)
					TextLabel_3.Font = Enum.Font.Ubuntu;
					TextLabel_3.Text = text;
					TextLabel_3.TextStrokeTransparency = 0.000;
					TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel_3.TextSize = 10.000;
					TextLabel_3.TextXAlignment = Enum.TextXAlignment.Left;
					Button.MouseButton1Down:Connect(function()
						Drop.Visible = not Drop.Visible;
						if not Drop.Visible then
							Drop.CanvasPosition = Vector2.new(0, 0)
						end
					end)
					local indrop = false;
					local ind = false;
					Drop.MouseEnter:Connect(function()
						indrop = true
					end)
					Drop.MouseLeave:Connect(function()
						indrop = false
					end)
					Button.MouseEnter:Connect(function()
						ind = true
					end)
					Button.MouseLeave:Connect(function()
						ind = false
					end)
					game:GetService("UserInputService").InputBegan:Connect(function(input)
						if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.MouseButton2 then
							if Drop.Visible == true and not indrop and not ind then
								Drop.Visible = false;
								Drop.CanvasPosition = Vector2.new(0, 0)
							end
						end
					end)
					values[tabname][sectorname][text] = Element.value
				elseif type == "Slider" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 25)
					local Slider = Instance.new("Frame")
					local TextLabel = Instance.new("TextLabel")
					local Button = Instance.new("TextButton")
					local Frame = Instance.new("Frame")
					local UIGradient = Instance.new("UIGradient")
					local UIGradient2 = Instance.new("UIGradient")
					local Value = Instance.new("TextLabel")
					Slider.Name = "Slider"
					Slider.Parent = Inner;
					Slider.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Slider.BackgroundTransparency = 1.000;
					Slider.Position = UDim2.new(0, 0, 0.653061211, 0)
					Slider.Size = UDim2.new(1, 0, 0, 25)
					TextLabel.Parent = Slider;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.Position = UDim2.new(0, 32, 0, -2)
					TextLabel.Size = UDim2.new(0, 100, 0, 15)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.Text = text;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					TextLabel.TextXAlignment = Enum.TextXAlignment.Left;
					Button.Name = "Button"
					Button.Parent = Slider;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Button.Position = UDim2.new(0, 30, 0, 15)
					Button.Size = UDim2.new(0, 175, 0, 5)
					Button.AutoButtonColor = false;
					Button.Font = Enum.Font.Ubuntu;
					Button.Text = ""
					Button.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button.TextSize = 10.000;
					UIGradient2.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(49, 49, 49)),
						ColorSequenceKeypoint.new(0.50, Color3.fromRGB(42, 42, 42)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(33, 33, 32))
					}
					UIGradient2.Rotation = 90;
					UIGradient2.Parent = Button;
					Frame.Parent = Button;
					Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Frame.BorderSizePixel = 0;
					Frame.Size = UDim2.new(0.5, 0, 1, 0)
					UIGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(123, 81, 153)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(77, 39, 109))
					}
					UIGradient.Rotation = 90;
					UIGradient.Parent = Frame;
					Value.Name = "Value"
					Value.Parent = Slider;
					Value.TextStrokeTransparency = 0.000;
					Value.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Value.BackgroundTransparency = 1.000;
					Value.Position = UDim2.new(0, 30, 0, 15)
					Value.Size = UDim2.new(0, 175, 0, 5)
					Value.Font = Enum.Font.Ubuntu;
					Value.Text = "50"
					Value.TextColor3 = Color3.fromRGB(255, 255, 255)
					Value.TextSize = 10.000;
					local min, max, default = data.min or 0, data.max or 100, data.default or 0;
					Element.value = {
						Slider = default
					}
					function Element:SetValue(value)
						Element.value = value;
						local a;
						if min > 0 then
							a = ((Element.value.Slider - min)) / (max - min)
						else
							a = (Element.value.Slider - min) / (max - min)
						end;
						Value.Text = Element.value.Slider;
						Frame.Size = UDim2.new(a, 0, 1, 0)
						values[tabname][sectorname][text] = Element.value;
						callback(value)
					end;
					local a;
					if min > 0 then
						a = ((Element.value.Slider - min)) / (max - min)
					else
						a = (Element.value.Slider - min) / (max - min)
					end;
					Value.Text = Element.value.Slider;
					Frame.Size = UDim2.new(a, 0, 1, 0)
					values[tabname][sectorname][text] = Element.value;
					local uis = game:GetService("UserInputService")
					local mouse = game.Players.LocalPlayer:GetMouse()
					local val;
					Button.MouseButton1Down:Connect(function()
						Frame.Size = UDim2.new(0, math.clamp(mouse.X - Frame.AbsolutePosition.X, 0, 175), 0, 5)
						val = math.floor((((tonumber(max) - tonumber(min)) / 175) * Frame.AbsoluteSize.X) + tonumber(min)) or 0;
						Value.Text = val;
						Element.value.Slider = val;
						values[tabname][sectorname][text] = Element.value;
						callback(Element.value)
						moveconnection = mouse.Move:Connect(function()
							Frame.Size = UDim2.new(0, math.clamp(mouse.X - Frame.AbsolutePosition.X, 0, 180), 0, 5)
							val = math.floor((((tonumber(max) - tonumber(min)) / 175) * Frame.AbsoluteSize.X) + tonumber(min))
							Value.Text = val;
							Element.value.Slider = val;
							values[tabname][sectorname][text] = Element.value;
							callback(Element.value)
						end)
						releaseconnection = uis.InputEnded:Connect(function(Mouse)
							if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
								Frame.Size = UDim2.new(0, math.clamp(mouse.X - Frame.AbsolutePosition.X, 0, 175), 0, 5)
								val = math.floor((((tonumber(max) - tonumber(min)) / 175) * Frame.AbsoluteSize.X) + tonumber(min))
								values[tabname][sectorname][text] = Element.value;
								callback(Element.value)
								moveconnection:Disconnect()
								releaseconnection:Disconnect()
							end
						end)
					end)
				elseif type == "Button" then
					Section.Size = Section.Size + UDim2.new(0, 0, 0, 24)
					local Button = Instance.new("Frame")
					local Button_2 = Instance.new("TextButton")
					local TextLabel = Instance.new("TextLabel")
					local UIGradient = Instance.new("UIGradient")
					Button.Name = "Button"
					Button.Parent = Inner;
					Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button.BackgroundTransparency = 1.000;
					Button.Position = UDim2.new(0, 0, 0.236059487, 0)
					Button.Size = UDim2.new(1, 0, 0, 24)
					Button_2.Name = "Button"
					Button_2.Parent = Button;
					Button_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					Button_2.BorderColor3 = Color3.fromRGB(18, 18, 16)
					Button_2.Position = UDim2.new(0, 30, 0.5, -9)
					Button_2.Size = UDim2.new(0, 175, 0, 18)
					Button_2.AutoButtonColor = false;
					Button_2.Font = Enum.Font.Ubuntu;
					Button_2.Text = ""
					Button_2.TextColor3 = Color3.fromRGB(0, 0, 0)
					Button_2.TextSize = 10.000;
					UIGradient.Color = ColorSequence.new{
						ColorSequenceKeypoint.new(0.00, Color3.fromRGB(46, 43, 44)),
						ColorSequenceKeypoint.new(1.00, Color3.fromRGB(25, 24, 24))
					}
					UIGradient.Rotation = 90;
					UIGradient.Parent = Button_2;
					TextLabel.Parent = Button_2;
					TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.BackgroundTransparency = 1.000;
					TextLabel.BorderColor3 = Color3.fromRGB(18, 18, 16)
					TextLabel.Size = UDim2.new(1, 0, 1, 0)
					TextLabel.Font = Enum.Font.Ubuntu;
					TextLabel.Text = text;
					TextLabel.TextStrokeTransparency = 0.000;
					TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
					TextLabel.TextSize = 10.000;
					function Element:SetValue()
					end;
					Button_2.MouseButton1Down:Connect(function()
						TextLabel.TextColor3 = Color3.fromRGB(97, 59, 227)
						library:Tween(TextLabel, TweenInfo.new(0.4, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
							TextColor3 = Color3.fromRGB(109, 57, 142)
						})
						callback()
					end)
					Button_2.MouseEnter:Connect(function()
						library:Tween(TextLabel, TweenInfo.new(0.2, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
							TextColor3 = Color3.fromRGB(124, 81, 149)
						})
					end)
					Button_2.MouseLeave:Connect(function()
						library:Tween(TextLabel, TweenInfo.new(0.2, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
							TextColor3 = Color3.fromRGB(255, 255, 255)
						})
					end)
				end;
				ConfigLoad:Connect(function(cfg)
					pcall(function()
						local fix = library:ConfigFix(cfg)
						if fix[tabname][sectorname][text] ~= nil then
							Element:SetValue(fix[tabname][sectorname][text])
						end
					end)
				end)
				return Element
			end;
			return Sector
		end;
		return Tab
	end;
	floppa.Parent = game.CoreGui;
	return menu
end;