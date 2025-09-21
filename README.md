use context dcic2024
include image
include math

# Problem 1
fun tick(s :: Number) -> Number:
  doc: "Given seconds 0..59, return the next second (59 -> 0)."
  if s == 59:
    0
  else:
    s + 1
  end
where:
  tick(0) is 1
  tick(1) is 2
  tick(58) is 59
  tick(59) is 0
end