# One-shot prompt: "Vaccines for kids and puppies" animation

Copy everything in the block below into a new chat. If you want the puppy to look like your own dog, attach a couple of photos of the dog along with it.

```
Create a single self-contained HTML file (inline SVG + CSS + vanilla JS, no external libraries
or images) that plays a short, gentle animation for young children. The goal: show a child that
just like kids need vaccines, dogs need them too.

STORY (plays once, about 31 seconds, then stops; a "↻ Watch again" button below replays it from
the start, resetting everything instantly with no glitches):
Scene 1 – a girl named Maya sits on an exam bench. A nurse approaches, gives a quick shot in
  Maya's upper arm (below a rolled-up sleeve), steps back, a bandage with a star appears, then
  a green "protected" shield with a check mark pops in.
Scene 2 – Stella, an Australian Shepherd puppy, sits on a vet's exam table. A vet does the same
  steps: approach, quick shot in the shoulder, step back, paw-print bandage, floating hearts,
  shield.
No page title and no end card – just the visual, a caption bar under it, and the replay button.

CAPTIONS (one line per beat, simple words for a 4–7 year old):
"This is Maya. Today is her vaccine day!" / "The doctor uses a tiny, tiny needle." /
"Pinch! It is over super fast." / "All done! Maya was so brave. A bandage and a sticker!" /
"The vaccine teaches her body to fight germs, so she stays healthy." /
"Dogs need vaccines too! This is Stella, an Australian Shepherd puppy." /
"The vet gives Stella a tiny pinch, just like Maya got." / "Yip! Quick pinch..." /
"All done! Good pup, Stella! A paw-print bandage!" / "Now Stella is protected from germs too."
Small speech bubbles: Maya "Pinch! Quick!" then "That wasn't so bad!"; Stella "Yip! Pinch!"
then "Woof! I'm brave!". Faces react: calm → a little worried → squeezed-shut eyes and an "o"
mouth at the pinch → big smile after.

CHARACTERS – life-like, not chibi:
- Real proportions: adults about 6.5 heads tall and clearly larger than the child; Maya has a
  child's proportions.
- Heads are sculpted shapes, never plain circles. Adults are in 3/4 view facing the patient:
  rounded skull, forehead, brow, cheekbone, jaw tapering to a chin, and exactly ONE nose that
  is part of the head outline (so it shares the face's shading – no separate nose shape, no
  extra nose lines). Maya has a soft oval face, full cheeks, small rounded chin, ears peeking
  out of her hair.
- Real eyes (whites, coloured irises, pupils, catchlights, upper lids), eyebrows, noses, lips.
- Maya clearly reads as a girl: long brown hair with bangs and side locks, a pink bow,
  eyelashes, pink top with a small heart, pleated purple skirt, pink Mary Jane shoes. She sits
  with arms relaxed, elbows bent, hands resting palm-down on her lap.
- Nurse: white lab coat over teal scrubs, nurse cap, dark hair in a bun. Vet: teal coat over a
  white shirt, stethoscope, short brown hair. Both have a long coat, legs and shoes on the floor.
- Stella (match the attached photos if provided): black tricolor Aussie puppy – black coat; tan
  eyebrow dots, cheeks, muzzle sides, lower legs and inner ears; white chest bib and white paws;
  brown eyes; soft ears that fold over and flop down beside the face; long black tail that wags
  (faster when happy); blue collar with a buckle; a realistic nose with nostrils.

ARMS AND HANDS (important – get these right):
- Each arm is two segments with fixed lengths (upper arm ≈ 62, forearm ≈ 58 in an 800×450
  viewBox). Drive the working arm with two-bone inverse kinematics from a fixed shoulder to the
  hand every animation frame. The arm must NEVER stretch or shrink in any frame, including
  during the plunger push, the return to rest, and the replay reset. Choose the elbow bend
  side that is anatomically natural for a 3/4 view (elbow back and down while reaching).
- Animate poses by blending the HAND position and syringe angle (not the needle tip), and keep
  every pose within reach.
- Relaxed pose: arm hanging naturally at the side with a slight bend, hand at hip height,
  syringe held low and pointing down. A hanging hand is NOT palm-out: show it side-on, palm
  toward the thigh, fingers together and gently curled, thumb lying along the index finger.
- The other arm hangs relaxed with the same bone lengths and a gentle sway.
- Syringe held in a dart grip, as for a real injection: the back of the hand above the barrel,
  the index finger lying along the top of the barrel in three jointed segments with a nail on
  the tip, the thumb along the near side of the barrel, and the middle, ring and little fingers
  curled underneath. The plunger end sticks out behind the hand.
- Hands MUST connect smoothly to the arms: the coat sleeve ends in a cuff, and a skin-coloured
  wrist runs from inside the cuff into the back of the hand, the same width as the hand where
  they meet, with no outline seam across the join.
- Every human hand has a palm, four fingers and a thumb, and every finger stays anatomically
  correct in every pose: jointed segments, correct lengths (middle longest, little shortest),
  bending only the way real fingers bend, never splayed or rubbery.
- Hands are sized to their arms: about as wide as the wrist and roughly 3/4 the length of the
  forearm. Maya's hands must not look tiny next to her arms.

LOOK – shading and texture on everything:
- Rooms: soft gradient walls with subtle wallpaper texture, a window with sky and daylight
  falling across the floor, wooden floor planks, white baseboards, a framed poster (pink cross
  / paw print) with a drop shadow, a metal bench / exam table with highlights, soft cast
  shadows under people, furniture and the puppy.
- People: shaded skin (radial gradients), shaded hair with strand highlights and slightly
  fuzzy edges, coats with a fabric weave, fold lines and sleeve highlights, shaded trousers
  and shoes.
- Stella: shaded fur gradients, a fine fur-strand texture, fuzzy fur edges (SVG turbulence +
  displacement filter), fluffy cheek tufts and a fluffy bottom edge on the bib.
- Props: glossy syringe glass with pink liquid that decreases when the plunger is pressed,
  shaded bandages, gradient shield with a highlight, speech bubbles with soft shadows.
- Calm, friendly palette; gentle idle motion (breathing, ear bob, arm sway, tail wag); respect
  prefers-reduced-motion.

LAYOUT: centered card that scales to the window width, caption bar under the picture,
pill-shaped pink "↻ Watch again" button below.

Before you finish, verify in a headless browser: take screenshots at several moments in both
scenes, zoom in on faces and hands, and measure the drawn upper-arm and forearm lengths every
frame for a full run to prove they never change.
```
