
# Godot Reference

## Tween

```
Sprite Shadow = (Sprite)Target.FindNode("Shadow");
Tween ShadowAlpha = new Tween { Name = "ShadowAlpha" };
Shadow.Modulate = new Color(1, 1, 1, 0);
ShadowAlpha.InterpolateProperty(
    Shadow, "modulate", new Color(1, 1, 1, 0), new Color(1, 1, 1, 1), Duration, Tween.TransitionType.Linear, Tween.EaseType.InOut, 0f
);
Shadow.AddChild(ShadowAlpha);
ShadowAlpha.Start();
```
