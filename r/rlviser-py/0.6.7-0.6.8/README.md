# Comparing `tmp/rlviser_py-0.6.7.tar.gz` & `tmp/rlviser_py-0.6.8.tar.gz`

## Comparing `rlviser_py-0.6.7.tar` & `rlviser_py-0.6.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.7/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/LICENSE
--rw-r--r--   0     1001      127     1557 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/README.md
--rw-r--r--   0     1001      127     2907 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/gym_renderer.py
--rw-r--r--   0     1001      127     2547 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/pygymtest.py
--rw-r--r--   0     1001      127     2291 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/rlviser_py.pyi
--rw-r--r--   0     1001      127    18232 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/src/bytes.rs
--rw-r--r--   0     1001      127     5195 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/src/lib.rs
--rw-r--r--   0     1001      127     5462 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/src/socket.rs
--rw-r--r--   0     1001      127     8092 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/Cargo.lock
--rw-r--r--   0     1001      127      387 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.8/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/LICENSE
+-rw-r--r--   0     1001      127     1557 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/README.md
+-rw-r--r--   0     1001      127     2854 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/gym_renderer.py
+-rw-r--r--   0     1001      127     2392 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/pygymtest.py
+-rw-r--r--   0     1001      127     2408 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/rlviser_py.pyi
+-rw-r--r--   0     1001      127    18232 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/src/bytes.rs
+-rw-r--r--   0     1001      127     5195 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/src/lib.rs
+-rw-r--r--   0     1001      127     5991 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/src/socket.rs
+-rw-r--r--   0     1001      127     8092 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/Cargo.lock
+-rw-r--r--   0     1001      127      387 2024-05-20 08:40:03.000000 rlviser_py-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.8/PKG-INFO
```

### Comparing `rlviser_py-0.6.7/Cargo.toml` & `rlviser_py-0.6.8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlviser-py"
-version = "0.6.7"
+version = "0.6.8"
 edition = "2021"
 description = "Python implementation that manages a UDP connection to RLViser"
 license = "MIT"
 repository = "https://github.com/VirxEC/rlviser-py"
 readme = "README.md"
 keywords = ["rlviser", "rocket-league", "udp", "python", "rlbot"]
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore"]
```

### Comparing `rlviser_py-0.6.7/LICENSE` & `rlviser_py-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.7/README.md` & `rlviser_py-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.7/gym_renderer.py` & `rlviser_py-0.6.8/gym_renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-from typing import Any, Dict
+from typing import Any
 
 import rlviser_py as rlviser
 import RocketSim as rsim
 from rlgym.api import Renderer
 from rlgym.rocket_league.api import Car, GameState
 from rlgym.rocket_league.common_values import BOOST_LOCATIONS
 
 
 class RLViserRenderer(Renderer[GameState]):
-
-    def __init__(self, tick_rate=120/8):
+    def __init__(self, tick_rate=120 / 8):
         rlviser.set_boost_pad_locations(BOOST_LOCATIONS)
         self.tick_rate = tick_rate
         self.packet_id = 0
 
-    def render(self, state: GameState, shared_info: Dict[str, Any]) -> Any:
+    def render(self, state: GameState, shared_info: dict[str, Any]) -> Any:
         boost_pad_states = [bool(timer == 0) for timer in state.boost_pad_timers]
 
         ball = rsim.BallState()
         ball.pos = rsim.Vec(*state.ball.position)
         ball.vel = rsim.Vec(*state.ball.linear_velocity)
         ball.ang_vel = rsim.Vec(*state.ball.angular_velocity)
-        # ball.rot_mat = rsim.RotMat(*state.ball.rotation_mtx.transpose().flatten())
+        ball.rot_mat = rsim.RotMat(*state.ball.rotation_mtx.transpose().flatten())
 
         car_data = []
         for idx, car in enumerate(state.cars.values()):
             car_state = self._get_car_state(car)
-            car_data.append((idx + 1, car.team_num, rsim.CarConfig(car.hitbox_type), car_state))
+            car_data.append(
+                (idx + 1, car.team_num, rsim.CarConfig(car.hitbox_type), car_state)
+            )
 
         self.packet_id += 1
-        rlviser.render(tick_count=self.packet_id, tick_rate=self.tick_rate, game_mode=rsim.GameMode.SOCCAR,
-                       boost_pad_states=boost_pad_states, ball=ball, cars=car_data)
+        rlviser.render(
+            tick_count=self.packet_id,
+            tick_rate=self.tick_rate,
+            game_mode=rsim.GameMode.SOCCAR,
+            boost_pad_states=boost_pad_states,
+            ball=ball,
+            cars=car_data,
+        )
 
     def close(self):
         rlviser.quit()
 
     # I stole this from RocketSimEngine
     def _get_car_state(self, car: Car):
         car_state = rsim.CarState()
@@ -42,15 +49,14 @@
         car_state.vel = rsim.Vec(*car.physics.linear_velocity)
         car_state.ang_vel = rsim.Vec(*car.physics.angular_velocity)
         car_state.rot_mat = rsim.RotMat(*car.physics.rotation_mtx.transpose().flatten())
 
         car_state.demo_respawn_timer = car.demo_respawn_timer
         car_state.is_on_ground = car.on_ground
         car_state.supersonic_time = car.supersonic_time
-        # print(car.boost_amount)
         car_state.boost = car.boost_amount * 100
         car_state.time_spent_boosting = car.boost_active_time
         car_state.handbrake_val = car.handbrake
 
         car_state.has_jumped = car.has_jumped
         car_state.last_controls.jump = car.is_holding_jump
         car_state.is_jumping = car.is_jumping
@@ -62,11 +68,8 @@
         car_state.flip_time = car.flip_time
         car_state.flip_rel_torque = rsim.Vec(*car.flip_torque)
 
         car_state.is_auto_flipping = car.is_autoflipping
         car_state.auto_flip_timer = car.autoflip_timer
         car_state.auto_flip_torque_scale = car.autoflip_direction
 
-        if car.bump_victim_id is not None:
-            car_state.car_contact_id = car.bump_victim_id
-
         return car_state
```

### Comparing `rlviser_py-0.6.7/pygymtest.py` & `rlviser_py-0.6.8/pygymtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,44 +25,42 @@
 if __name__ == "__main__":
     game_speed = 1
 
     env = RLGym(
         state_mutator=MutatorSequence(
             FixedTeamSizeMutator(blue_size=2, orange_size=2), KickoffMutator()
         ),
-        obs_builder=DefaultObs(zero_padding=None),
-        action_parser=RepeatAction(LookupTableAction(), repeats=1),
+        obs_builder=DefaultObs(zero_padding=2),
+        action_parser=RepeatAction(LookupTableAction()),
         reward_fn=CombinedReward((GoalReward(), 10.0), (TouchReward(), 0.1)),
         termination_cond=GoalCondition(),
         truncation_cond=AnyCondition(
             TimeoutCondition(timeout=300.0), NoTouchTimeoutCondition(timeout=30.0)
         ),
         transition_engine=RocketSimEngine(),
-        renderer=RLViserRenderer(120),
+        renderer=RLViserRenderer(),
     )
 
     # simulate 2 episodes
     for _ in range(2):
         obs_dict = env.reset()
         steps = 0
         ep_reward = {agent_id: 0.0 for agent_id in env.agents}
         t0 = time.time()
         while True:
             actions = {}
-            for agent_id, action_space in env.action_spaces.items():
-                # agent.act(obs) | Your agent should go here
-                actions[agent_id] = np.random.randint(action_space, size=(1,))
-
-            for _ in range(8):
-                obs_dict, reward_dict, terminated_dict, truncated_dict = env.step(
-                    actions
-                )
-                env.render()
-                time.sleep(max(0, t0 + steps / (120 * game_speed) - time.time()))
-                steps += 1
+            for agent_id, (type, action_spaces) in env.action_spaces.items():
+                actions[agent_id] = np.random.randint(action_spaces, size=(1,))
+
+            obs_dict, reward_dict, terminated_dict, truncated_dict = env.step(
+                actions
+            )
+            env.render()
+            time.sleep(15 / 120 / game_speed)
+            steps += 1
 
             for agent_id, reward in reward_dict.items():
                 ep_reward[agent_id] += reward
 
             if any(chain(terminated_dict.values(), truncated_dict.values())):
                 break
```

### Comparing `rlviser_py-0.6.7/rlviser_py.pyi` & `rlviser_py-0.6.8/rlviser_py.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Sequence, Optional, Tuple
+from typing import Sequence, Optional
 
-from RocketSim import BallState, CarState, GameMode
+from RocketSim import BallState, CarState, GameMode, CarConfig
 
-type TVec3 = Tuple[float, float, float]
+type TVec3 = tuple[float, float, float]
 """
 The items are (X, Y, Z) respectively
 """
-type TRotmat = Tuple[TVec3, TVec3, TVec3]
+type TRotmat = tuple[TVec3, TVec3, TVec3]
 """
 The items are (forward, right, up) respectively
 """
-type TBall = Tuple[TVec3, TRotmat, TVec3, TVec3]
+type TBall = tuple[TVec3, TRotmat, TVec3, TVec3]
 """
 The items are (location, rotation, velocity, angular velocity) respectively
 """
-type TCar = Tuple[int, TVec3, TRotmat, TVec3, TVec3, float, bool, bool, bool, float]
+type TCar = tuple[int, TVec3, TRotmat, TVec3, TVec3, float, bool, bool, bool, float]
 """
 The items are (car_id, location, rotation, velocity, angular velocity, boost, has jumped, has double jumped, has flipped, demo respawn timer) respectively
 """
 
 def set_boost_pad_locations(locations: Sequence[TVec3]) -> ...:
     pass
 
-def get_state_set() -> Optional[Tuple[Sequence[float], TBall, Sequence[TCar]]]:
+def get_state_set() -> Optional[tuple[Sequence[float], TBall, Sequence[TCar]]]:
     """
     Sequence[float] - Boost pad states, 0 for full and some positive value for the time in seconds until it respawns
     TBall - Ball state
     Sequence[TCar] - Car states
     """
     pass
 
@@ -57,12 +57,17 @@
     """
     Reports the current game pause state to RLViser. This is used to update the game pause state in the UI.
 
     NOTE: This is only needed when RLViser did not request the game pause state change.
     """
     pass
 
-def render(tick_count: int, tick_rate: float, game_mode: GameMode, boost_pad_states: Sequence[bool], ball: BallState, cars: Sequence[Tuple[int, CarState]]) -> ...:
+type CarData = tuple[int, int, CarConfig, CarState]
+"""
+The items are (car_id, team, car_config, car_state) respectively
+"""
+
+def render(tick_count: int, tick_rate: float, game_mode: GameMode, boost_pad_states: Sequence[bool], ball: BallState, cars: Sequence[CarData]) -> ...:
     pass
 
 def quit() -> ...:
     pass
```

### Comparing `rlviser_py-0.6.7/src/bytes.rs` & `rlviser_py-0.6.8/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.7/src/lib.rs` & `rlviser_py-0.6.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.7/src/socket.rs` & `rlviser_py-0.6.8/src/socket.rs`

 * *Files 7% similar despite different names*

```diff
@@ -87,15 +87,29 @@
             let Some(packet_type) = UdpPacketTypes::new(byte_buffer[0]) else {
                 println!("Received unknown packet type: {}", byte_buffer[0]);
                 break;
             };
 
             match packet_type {
                 UdpPacketTypes::GameState => {
-                    self.socket.peek_from(&mut min_game_state_buf)?;
+                    #[cfg(windows)]
+                    {
+                        while let Err(e) = self.socket.peek_from(&mut min_game_state_buf) {
+                            if let Some(code) = e.raw_os_error() {
+                                if code == 10040 {
+                                    break;
+                                }
+                            }
+                        }
+                    }
+
+                    #[cfg(not(windows))]
+                    {
+                        while self.socket.peek_from(&mut min_game_state_buf).is_err() {}
+                    }
 
                     let num_bytes = GameState::get_num_bytes(&min_game_state_buf);
                     game_state_buffer.resize(num_bytes, 0);
                     self.socket.recv_from(&mut game_state_buffer)?;
 
                     game_state = Some(GameState::from_bytes(&game_state_buffer));
                 }
```

### Comparing `rlviser_py-0.6.7/Cargo.lock` & `rlviser_py-0.6.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -90,17 +90,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -180,15 +180,15 @@
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.6.7"
+version = "0.6.8"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -199,17 +199,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.64"
+version = "2.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ad3dee41f36859875573074334c200d1add8e4a87bb37113ebd31d926b7b11f"
+checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `rlviser_py-0.6.7/PKG-INFO` & `rlviser_py-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlviser-py
-Version: 0.6.7
+Version: 0.6.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

