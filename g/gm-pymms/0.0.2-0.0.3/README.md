# Comparing `tmp/gm_pymms-0.0.2.tar.gz` & `tmp/gm_pymms-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gm_pymms-0.0.2.tar", last modified: Thu Feb 29 20:43:32 2024, max compression
+gzip compressed data, was "gm_pymms-0.0.3.tar", last modified: Fri Apr 19 02:10:53 2024, max compression
```

## Comparing `gm_pymms-0.0.2.tar` & `gm_pymms-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 20:43:32.362978 gm_pymms-0.0.2/
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    35149 2024-02-26 08:45:54.000000 gm_pymms-0.0.2/LICENSE
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      576 2024-02-29 20:43:32.362978 gm_pymms-0.0.2/PKG-INFO
--rw-------   0 u0_a237  (10237) u0_a237  (10237)       54 2024-02-29 18:30:15.000000 gm_pymms-0.0.2/README.md
-drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 20:43:32.362978 gm_pymms-0.0.2/gm_pymms/
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      519 2024-02-26 08:45:54.000000 gm_pymms-0.0.2/gm_pymms/Timer.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/gm_pymms/__init__.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)     4821 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/gm_pymms/driver_audio.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)     1607 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/gm_pymms/driver_sounddevice_audio.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)     2524 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/gm_pymms/driver_termux_audio.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    17480 2024-02-29 20:43:31.000000 gm_pymms-0.0.2/gm_pymms/pymms
--rw-------   0 u0_a237  (10237) u0_a237  (10237)     5989 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/gm_pymms/pymms.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    31704 2024-02-26 08:45:54.000000 gm_pymms-0.0.2/gm_pymms/termcontrol.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    17480 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/gm_pymms/termplayer.py
-drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 20:43:32.362978 gm_pymms-0.0.2/gm_pymms.egg-info/
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      576 2024-02-29 20:43:32.000000 gm_pymms-0.0.2/gm_pymms.egg-info/PKG-INFO
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      423 2024-02-29 20:43:32.000000 gm_pymms-0.0.2/gm_pymms.egg-info/SOURCES.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)        1 2024-02-29 20:43:32.000000 gm_pymms-0.0.2/gm_pymms.egg-info/dependency_links.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)       21 2024-02-29 20:43:32.000000 gm_pymms-0.0.2/gm_pymms.egg-info/requires.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)        9 2024-02-29 20:43:32.000000 gm_pymms-0.0.2/gm_pymms.egg-info/top_level.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      162 2024-02-29 18:49:20.000000 gm_pymms-0.0.2/pyproject.toml
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      564 2024-02-29 20:43:32.366978 gm_pymms-0.0.2/setup.cfg
--rwx------   0 u0_a237  (10237) u0_a237  (10237)      706 2024-02-29 20:43:17.000000 gm_pymms-0.0.2/setup.py
+drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-04-19 02:10:53.855636 gm_pymms-0.0.3/
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)    35149 2024-02-26 08:45:54.000000 gm_pymms-0.0.3/LICENSE
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      576 2024-04-19 02:10:53.855636 gm_pymms-0.0.3/PKG-INFO
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)       54 2024-02-29 18:30:15.000000 gm_pymms-0.0.3/README.md
+drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-04-19 02:10:53.851636 gm_pymms-0.0.3/gm_pymms/
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      519 2024-02-26 08:45:54.000000 gm_pymms-0.0.3/gm_pymms/Timer.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 20:43:17.000000 gm_pymms-0.0.3/gm_pymms/__init__.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)     4821 2024-04-06 05:46:10.000000 gm_pymms-0.0.3/gm_pymms/driver_audio.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)     1699 2024-04-14 04:22:22.000000 gm_pymms-0.0.3/gm_pymms/driver_sounddevice_audio.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)     2797 2024-04-14 04:22:22.000000 gm_pymms-0.0.3/gm_pymms/driver_termux_audio.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)     2792 2024-03-22 05:14:15.000000 gm_pymms-0.0.3/gm_pymms/noise_filter.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)    19769 2024-04-19 02:10:53.000000 gm_pymms-0.0.3/gm_pymms/pymms
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)     6160 2024-04-17 23:24:41.000000 gm_pymms-0.0.3/gm_pymms/pymms.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)    19769 2024-04-19 02:06:00.000000 gm_pymms-0.0.3/gm_pymms/termplayer.py
+drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-04-19 02:10:53.855636 gm_pymms-0.0.3/gm_pymms.egg-info/
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      576 2024-04-19 02:10:53.000000 gm_pymms-0.0.3/gm_pymms.egg-info/PKG-INFO
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      424 2024-04-19 02:10:53.000000 gm_pymms-0.0.3/gm_pymms.egg-info/SOURCES.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)        1 2024-04-19 02:10:53.000000 gm_pymms-0.0.3/gm_pymms.egg-info/dependency_links.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)       21 2024-04-19 02:10:53.000000 gm_pymms-0.0.3/gm_pymms.egg-info/requires.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)        9 2024-04-19 02:10:53.000000 gm_pymms-0.0.3/gm_pymms.egg-info/top_level.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      162 2024-02-29 18:49:20.000000 gm_pymms-0.0.3/pyproject.toml
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      564 2024-04-19 02:10:53.855636 gm_pymms-0.0.3/setup.cfg
+-rwx------   0 u0_a237  (10237) u0_a237  (10237)      706 2024-04-19 02:06:00.000000 gm_pymms-0.0.3/setup.py
```

### Comparing `gm_pymms-0.0.2/LICENSE` & `gm_pymms-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gm_pymms-0.0.2/PKG-INFO` & `gm_pymms-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gm_pymms
-Version: 0.0.2
+Version: 0.0.3
 Summary: python xmms inspired media player/recorder
 Home-page: https://github.com/gretchycat/pymms
 Author: Gretchen Maculo
 Author-email: gretchen.maculo@gmail.com
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gm_pymms-0.0.2/gm_pymms/Timer.py` & `gm_pymms-0.0.3/gm_pymms/Timer.py`

 * *Files identical despite different names*

### Comparing `gm_pymms-0.0.2/gm_pymms/driver_audio.py` & `gm_pymms-0.0.3/gm_pymms/driver_audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .Timer import Timer
-
+import math
 from pydub import AudioSegment
+from .noise_filter import noise_reduction
 
 STOP=0
 PLAY=1
 RECORD=2
 
 class driver_audio():
     def __init__(self):
@@ -20,28 +21,27 @@
         self.audio_start=0
         self.record_audio=None
         return None
 
     def load(self, filename):
         self.timer.clear()
         self.audio=AudioSegment.from_file(filename)
+        self.filename=filename
         self.setAudioProperties(fps=self.audio.frame_rate,
-            channels=self.audio.channels, sample_width=self.audio.sample_width)
+            channels=self.audio.channels, 
+            sample_width=self.audio.sample_width)
         self.audio_start=0
         return self.audio
 
     def play(self, start=0, end=0):
         self.status=PLAY
-        #buffer=self.audio.get_array_of_samples()
         self.audio_start=self.get_cursor()
         self.timer.start(factor=self.audio.frame_rate, offset=-int(self.get_cursor()/self.audio.frame_rate))
         if end==0:
             pass
-            #return sd.play(buffer[int(start):], self.audio.frame_rate)
-        #return sd.play(buffer[int(start):int(end)], self.audio.frame_rate)
 
     def stop(self):
         #sd.stop()
         self.status=STOP
         if self.record_buffer is not None:
             frames=int(self.timer.get())
             self.record_audio=self.setAudio(self.record_buffer[:frames],
@@ -143,13 +143,16 @@
         elif sf is not None:
             clip_frames=self.audio.get_array_of_samples()[sf:]
         elif ef is not None:
             clip_frames=self.audio.get_array_of_samples()[:ef]
         else:
             clip_frames=self.audio.get_array_of_samples()
         #convert to AudioSegment
-        audio_segment = AudioSegment(clip_frames.tobytes(), frame_rate=fps, 
+        audio_segment = AudioSegment(clip_frames.tobytes(), frame_rate=fps,
             sample_width=sample_width, channels=channels)
         if audio_segment.frame_count()>0:
             return audio_segment
         return None
 
+    def noiseFilter(self):
+        filtered_segment = noise_reduction(self.audio, smooth_factor=0.2)
+
```

### Comparing `gm_pymms-0.0.2/gm_pymms/driver_sounddevice_audio.py` & `gm_pymms-0.0.3/gm_pymms/driver_sounddevice_audio.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,18 @@
     def __init__(self):
         super().__init__()
 
     def play(self, start=0, end=0):
         super().play(start=start, end=end)
         buffer=self.audio.get_array_of_samples()
         if end==0:
-            return sd.play(buffer[int(start):], self.audio.frame_rate)
-        return sd.play(buffer[int(start):int(end)], self.audio.frame_rate)
+            return sd.play(buffer[int(start):],
+                           samplerate=self.audio.frame_rate*self.audio.channels)
+        return sd.play(buffer[int(start):int(end)],
+                       samplerate=self.audio.frame_rate)
 
     def stop(self):
         sd.stop()
         super().stop()
 
     def rec(self):
         super().rec()
```

### Comparing `gm_pymms-0.0.2/gm_pymms/pymms` & `gm_pymms-0.0.3/gm_pymms/pymms`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,30 @@
 
 def minsec(s):
     s=int(s)
     mins=int(s/60)
     secs=int(s%60)
     return f'{mins:02d}:{secs:02d}'
 
+def scroll_string(str, max_length, clock=0):
+    max_index=len(str)-max_length
+    if max_index>0:
+        cl=0
+        cl=int(clock)%(2*max_index)
+        rv=0
+        if cl>max_index:
+            rv=cl-max_index
+        st=int(cl-2*rv)
+        return str[st:st+max_length]
+    return str
+
 class termplayer(widget):
-    def __init__(self, x=1, y=1, w=80, h=15, mode='play', files=[], script=""): 
+    def __init__(self, x=1, y=1, w=80, h=15, mode='play', files=[], script="",
+                 repeat=False, shuffle=False, play=False, playlist=False):
+        self.go=False
         self.icons={}
         self.icons['prev']     = {"label":'\u23ee',   "key":'[', 'action':self.prev}
         self.icons['prev']     = {"label":'\u25ae'+'\u25c0'*2, "key":'[', 'action':self.prev}
         self.icons['next']     = {"label":'\u23ed',   "key":']', 'action':self.next}
         self.icons['next']     = {"label":'\u25b6'*2+'\u25ae', "key":']', 'action':self.next}
         self.icons['play']     = {"label":'\u25b6',   "key":'P', 'action':self.play}
         self.icons['pause']    = {"label":'\u25ae'*2, "key":'p', 'action':self.pause}
@@ -60,15 +74,19 @@
         self.icons['quit']=      {"label":'Quit',     "key":'q', 'action':self.quit}
         super().__init__(x=x, y=y, w=w, h=h)
         self.showPlayList=False
         self.clearPlayList=False
         self.playlist=files
         self.playlistinorder=files.copy()
         self.playListInfo={}
-        self.repeat=False
+        self.repeat=repeat
+        self.playlistbuffer=''
+        self.playerbuffer=''
+        if shuffle:
+            self.shuffle()
         self.mode=mode
         for f in files:
             self.playListInfo[f]=self.mediaInfo(f)
         if self.mode=='record':
             if len(self.playlist)!=1:
                 print("Record mode must reference one audio filename.")
                 exit(1)
@@ -82,43 +100,46 @@
         self.script=script
         self.frame=0
         self.anim="\\-/|"
         self.x=x
         self.y=y
         self.w=w
         self.h=h
+        sh=termcontrol.get_terminal_size(0)['rows']
         self.playerbox=widgetScreen(self.x, self.y, self.w, self.h, bg=234, fg=15, style='outside')
-        self.playlistbox=widgetScreen(self.x, self.y+self.h, self.w, self.h, bg=234, fg=15, style='outside')
+        self.playlistbox=widgetScreen(self.x, self.y+self.h, self.w, sh-self.h, bg=234, fg=15, style='outside')
         self.addWidget(self.playerbox)
         self.addWidget(self.playlistbox)
         boxHeight=7
         timeBoxW=30
         self.timeBox=widgetScreen(2, 1, timeBoxW, boxHeight, bg=233, fg=27, style='inside')
         self.playerbox.addWidget(self.timeBox)
         self.infoBox=widgetScreen(2+timeBoxW+2, 1, self.w-4-(timeBoxW+4), boxHeight, bg=233, fg=27, style='inside')
         self.playerbox.addWidget(self.infoBox)
         self.timeBox.box.tintFrame('#555')
         self.infoBox.box.tintFrame('#555')
         self.slider=widgetSlider(2, boxHeight+1, self.w-(2*2), 0, self.player.length(), labelType='time' , key='k')
         self.playerbox.addWidget(self.slider)
         self.addButtons(mode)
+        if play: self.play()
+        if playlist: self.togglePlayList()
 
     def addButtons(self,mode):
         playbuttons=['prev', 'play/pause', 'stop', 'next', '', 'shuffle', 'repeat', 'playlist', '', 'quit']
         recordbuttons=['seek-', 'play/pause', 'stop', 'record', 'seek+', '', 'denoise', 'normalize', '', 'quit']
         buttons=playbuttons
         if mode=='record':
             buttons=recordbuttons
-        else: 
+        else:
             buttons=playbuttons
         self.btn={}
         btnX=2
         btnY=10
         btnW=7
-        btnH=4 
+        btnH=4
         x=0
         for label in buttons:
             if self.icons.get(label):
                 i=self.icons[label]
                 toggle=None
                 if label in ['shuffle', 'playlist', 'repeat']:
                     if label=='shuffle':
@@ -128,15 +149,15 @@
                     if label=='repeat':
                         toggle=self.repeat
                 self.btn[label]=widgetButton(x*btnW+btnX, btnY, btnW, btnH, fg=27, bg=233, caption=i['label'], key=i['key'], action=i['action'], toggle=toggle)
                 self.playerbox.addWidget(self.btn[label])
             x+=1
 
     def mediaInfo(self, f):
-        title=f
+        title=os.path.basename(f)
         length=0
         bitrate=0
         quality=0
         channels=1
         info={'title':title, 'length':length, 'bitrate':bitrate, 'quality':quality, 'channels':channels}
         self.playListInfo[f]=info
         return info
@@ -234,23 +255,23 @@
             self.infoBox.feed(self.script)
             pass
         elif self.mode=='play':
             self.infoBox.feed(self.t.clear())
             self.infoBox.feed(self.t.ansicolor(27))
             title=""
             title=f'{self.playlist.index(self.filename)+1}. '
-            if self.playListInfo[self.filename]: 
+            if self.playListInfo[self.filename]:
                 title+=self.playListInfo[self.filename]['title']
                 title+=f' ({minsec(self.playListInfo[self.filename]["length"])})'
             self.infoBox.feed(self.t.gotoxy(1, 1))
-            self.infoBox.feed(title)
+            self.infoBox.feed(scroll_string(title, 38, clock=t))
             quality=0
             bitrate=0
             channels=0
-            if self.playListInfo[self.filename]: 
+            if self.playListInfo[self.filename]:
                 quality=int(self.playListInfo[self.filename]["quality"])
                 bitrate=int(self.playListInfo[self.filename]["bitrate"])
                 channels=int(self.playListInfo[self.filename]["channels"])
             self.infoBox.feed(self.t.gotoxy(1, 3))
             self.infoBox.feed(f'{int(quality)}kbps')
             self.infoBox.feed(self.t.gotoxy(14, 3))
             self.infoBox.feed(f'{bitrate}kHz')
@@ -289,55 +310,66 @@
         self.timeBox.feed(self.t.gotoxy(1, 4))
         self.timeBox.feed(self.t.ansicolor(rcolor, 233, bold=True))
         self.timeBox.feed(i['label'])
         i=self.icons['shuffle']
         self.timeBox.feed(self.t.gotoxy(1, 5))
         self.timeBox.feed(self.t.ansicolor(scolor, 233, bold=True))
         self.timeBox.feed(i['label'])
-        buffer+=self.playerbox.draw()
+        playerbuffer=self.playerbox.draw()
+        if playerbuffer!=self.playerbuffer:
+            buffer+=playerbuffer
+            self.playerbuffer=playerbuffer
         if self.showPlayList:
             self.playlistbox.feed(f'{self.t.clear()}')
             startline=self.playlist.index(self.filename)
-            if startline+self.h-3>len(self.playlist):
-                startline=len(self.playlist)-(self.h-2)
+            if startline+self.playlistbox.h-3>len(self.playlist):
+                startline=len(self.playlist)-(self.playlistbox.h-2)
             if startline<0:
                 startline=0
-            for n in range(self.h-2):
+            for n in range(self.playlistbox.h-2):
                 color=27
                 if n+startline<len(self.playlist):
                     f=self.playlist[startline+n]
                     if f==self.filename:
                         color=46
                     self.playlistbox.feed(f'{self.t.gotoxy(1,n+1)}')
                     self.playlistbox.feed(f'{self.t.ansicolor(color)}')
                     title=f
                     tm="00:00"
                     if self.playListInfo[f]:
                         title=f"{self.playListInfo[f]['title']}"
                         tm=f"{minsec(self.playListInfo[f]['length'])}"
-                    self.playlistbox.feed(f'{n+startline+1}. {title}')
-                    self.playlistbox.feed(f'{self.t.gotoxy(self.w-3-len(tm),n+1)}')
+                    else:
+                        title=os.path.basename(title)
+                    PL_line_length=self.playlistbox.w-4-len(f' {tm}')-len(f'{n+startline+1}. ')
+                    self.playlistbox.feed(f'{n+startline+1}. {scroll_string(title, PL_line_length, clock=0)}')
+                    self.playlistbox.feed(f'{self.t.gotoxy(self.playlistbox.w-3-len(tm), n+1)}')
                     self.playlistbox.feed(f'{tm}')
                 else:
-                    self.playlistbox.feed(f'{self.t.gotoxy(1,n+1)} ') 
-            buffer+=self.playlistbox.draw()
+                    self.playlistbox.feed(f'{self.t.gotoxy(1,n+1)} ')
+
+            playlistbuffer=self.playlistbox.draw()
+            if playlistbuffer!=self.playlistbuffer:
+                buffer+=playlistbuffer
+                self.playlistbuffer=playlistbuffer
         else:
             if self.clearPlayList:
                 self.clearPlayList=False
                 buffer+=self.t.reset()
-                for y in range(self.y+self.h,self.y+2*self.h):
+                for y in range(self.y+self.h,self.y+self.h+self.playlistbox.h):
                     buffer+=self.t.gotoxy(self.x, y)
                     for x in range(0, self.w):
                         buffer+=' '
         #print(self.anim[self.frame % len(self.anim)])
         self.frame +=1
         return buffer
 
     def togglePlayList(self):
         self.showPlayList=not self.showPlayList
+        self.playlistbuffer=''
         if not self.showPlayList:
             self.clearPlayList=True
 
     def load(self, filename):
         info=self.player.load(filename)
         self.playListInfo[filename]=info
         self.filename=filename
@@ -347,32 +379,38 @@
 
     def quit(self):
         if self.mode=='record':
             #TODO save prompt
             if(1):
                 self.save(self.filename)
         self.stop()
-        quit()
+        if self.go:
+            self.go=False
+        else:
+            pass
+            #quit()
 
     def next(self):
         i=self.playlist.index(self.filename)
         i+=1
         if i>=len(self.playlist):
             i=0
+        p=self.player.au.status
         self.load(self.playlist[i])
-        if self.mode=='play':
+        if p==PLAY:
             self.play()
 
     def prev(self):
         i=self.playlist.index(self.filename)
         i-=1
         if i<0:
             i=len(self.playlist)-1
+        p=self.player.au.status
         self.load(self.playlist[i])
-        if self.mode=='play':
+        if p==PLAY:
             self.play()
 
     def endHandler(self):
         if self.player.au.status==PLAY:
             if self.mode=='play':
                 if self.repeat:
                     self.stop()
@@ -422,29 +460,46 @@
         self.player.denoise()
 
     def normalize(self):
         self.player.normalize()
 
 def main():
     parser=OptionParser(usage="usage: %prog [options] AUDIO_FILES")
-    parser.add_option("-r", "--record", action='store_true', dest="record", 
+    parser.add_option("-p", "--play", action='store_true', dest="play",
+            default=False, help="Play immediately.")
+    parser.add_option("-r", "--record", action='store_true', dest="record",
             default=False, help="Record mode.")
+    parser.add_option("-S", "--shuffle", action='store_true', dest="shuffle",
+            default=False, help="Turn on shuffle.")
+    parser.add_option("-R", "--repeat", action='store_true', dest="repeat",
+            default=False, help="Turn on repeat.")
+    parser.add_option("-L", "--list", action='store_true', dest="playlist",
+            default=False, help="show playlist.")
     parser.add_option("-v", "--verbose", dest="debug", default="info",
             help="Show debug messages.[debug, info, warning]")
     parser.add_option("-s", dest="script", default="No script was given.",
             help="Script for record mode.")
-    parser.add_option("-x", dest="x", default=1, help="Top left coordinate.")
-    parser.add_option("-y", dest="y", default=1, help="Top left coordinate.")
-
+    parser.add_option("-x", dest="x", default=1, help="Left coordinate.")
+    parser.add_option("-y", dest="y", default=1, help="Top coordinate.")
     (options, args)=parser.parse_args()
     if len(args)==0:
         parser.print_help()
         return
     mode='play'
     if options.record:
         mode='record'
-    tp=termplayer(x=int(options.x), y=int(options.y), mode=mode, script=options.script, files=args)
+    tp=termplayer(x=int(options.x), y=int(options.y), mode=mode,
+                  script=options.script, files=args,
+                  shuffle=options.shuffle, repeat=options.repeat,
+                  play=options.play,
+                  playlist=options.playlist and not options.record)
+    tp.kb.disable_keyboard_echo()
+    print(tp.t.disable_cursor(), end='')
+    print(tp.t.disable_mouse(), end='')
     tp.guiLoop()
+    tp.kb.enable_keyboard_echo()
+    print(tp.t.enable_cursor(), end='')
+    print(tp.t.enable_mouse(), end='')
     return
 
 if __name__ == "__main__":
     main()
```

### Comparing `gm_pymms-0.0.2/gm_pymms/pymms.py` & `gm_pymms-0.0.3/gm_pymms/pymms.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,25 @@
         self.record_channels=1
         self.record_sample_width=16//8
         self.selected=0
         self.selected_length=0
         self.stop()
         self.au=au
 
+    def status(self):
+        if au.status==PLAY:
+            return 'play'
+        if au.status==RECORF:
+            return 'record'
+        return ''
+
     def load(self, filename):
         self.stop()
         audio=au.load(filename)
-        return {'title':filename, 'length':audio.duration_seconds, 
+        return {'title':os.path.basename(filename), 'length':audio.duration_seconds, 
                 'bitrate':audio.frame_rate, 'quality':audio.sample_width, 
                 'channels':audio.channels}
 
     def save(self, filename):
         return au.save(filename)
 
     def playpause(self):
```

### Comparing `gm_pymms-0.0.2/gm_pymms/termplayer.py` & `gm_pymms-0.0.3/gm_pymms/termplayer.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,30 @@
 
 def minsec(s):
     s=int(s)
     mins=int(s/60)
     secs=int(s%60)
     return f'{mins:02d}:{secs:02d}'
 
+def scroll_string(str, max_length, clock=0):
+    max_index=len(str)-max_length
+    if max_index>0:
+        cl=0
+        cl=int(clock)%(2*max_index)
+        rv=0
+        if cl>max_index:
+            rv=cl-max_index
+        st=int(cl-2*rv)
+        return str[st:st+max_length]
+    return str
+
 class termplayer(widget):
-    def __init__(self, x=1, y=1, w=80, h=15, mode='play', files=[], script=""): 
+    def __init__(self, x=1, y=1, w=80, h=15, mode='play', files=[], script="",
+                 repeat=False, shuffle=False, play=False, playlist=False):
+        self.go=False
         self.icons={}
         self.icons['prev']     = {"label":'\u23ee',   "key":'[', 'action':self.prev}
         self.icons['prev']     = {"label":'\u25ae'+'\u25c0'*2, "key":'[', 'action':self.prev}
         self.icons['next']     = {"label":'\u23ed',   "key":']', 'action':self.next}
         self.icons['next']     = {"label":'\u25b6'*2+'\u25ae', "key":']', 'action':self.next}
         self.icons['play']     = {"label":'\u25b6',   "key":'P', 'action':self.play}
         self.icons['pause']    = {"label":'\u25ae'*2, "key":'p', 'action':self.pause}
@@ -60,15 +74,19 @@
         self.icons['quit']=      {"label":'Quit',     "key":'q', 'action':self.quit}
         super().__init__(x=x, y=y, w=w, h=h)
         self.showPlayList=False
         self.clearPlayList=False
         self.playlist=files
         self.playlistinorder=files.copy()
         self.playListInfo={}
-        self.repeat=False
+        self.repeat=repeat
+        self.playlistbuffer=''
+        self.playerbuffer=''
+        if shuffle:
+            self.shuffle()
         self.mode=mode
         for f in files:
             self.playListInfo[f]=self.mediaInfo(f)
         if self.mode=='record':
             if len(self.playlist)!=1:
                 print("Record mode must reference one audio filename.")
                 exit(1)
@@ -82,43 +100,46 @@
         self.script=script
         self.frame=0
         self.anim="\\-/|"
         self.x=x
         self.y=y
         self.w=w
         self.h=h
+        sh=termcontrol.get_terminal_size(0)['rows']
         self.playerbox=widgetScreen(self.x, self.y, self.w, self.h, bg=234, fg=15, style='outside')
-        self.playlistbox=widgetScreen(self.x, self.y+self.h, self.w, self.h, bg=234, fg=15, style='outside')
+        self.playlistbox=widgetScreen(self.x, self.y+self.h, self.w, sh-self.h, bg=234, fg=15, style='outside')
         self.addWidget(self.playerbox)
         self.addWidget(self.playlistbox)
         boxHeight=7
         timeBoxW=30
         self.timeBox=widgetScreen(2, 1, timeBoxW, boxHeight, bg=233, fg=27, style='inside')
         self.playerbox.addWidget(self.timeBox)
         self.infoBox=widgetScreen(2+timeBoxW+2, 1, self.w-4-(timeBoxW+4), boxHeight, bg=233, fg=27, style='inside')
         self.playerbox.addWidget(self.infoBox)
         self.timeBox.box.tintFrame('#555')
         self.infoBox.box.tintFrame('#555')
         self.slider=widgetSlider(2, boxHeight+1, self.w-(2*2), 0, self.player.length(), labelType='time' , key='k')
         self.playerbox.addWidget(self.slider)
         self.addButtons(mode)
+        if play: self.play()
+        if playlist: self.togglePlayList()
 
     def addButtons(self,mode):
         playbuttons=['prev', 'play/pause', 'stop', 'next', '', 'shuffle', 'repeat', 'playlist', '', 'quit']
         recordbuttons=['seek-', 'play/pause', 'stop', 'record', 'seek+', '', 'denoise', 'normalize', '', 'quit']
         buttons=playbuttons
         if mode=='record':
             buttons=recordbuttons
-        else: 
+        else:
             buttons=playbuttons
         self.btn={}
         btnX=2
         btnY=10
         btnW=7
-        btnH=4 
+        btnH=4
         x=0
         for label in buttons:
             if self.icons.get(label):
                 i=self.icons[label]
                 toggle=None
                 if label in ['shuffle', 'playlist', 'repeat']:
                     if label=='shuffle':
@@ -128,15 +149,15 @@
                     if label=='repeat':
                         toggle=self.repeat
                 self.btn[label]=widgetButton(x*btnW+btnX, btnY, btnW, btnH, fg=27, bg=233, caption=i['label'], key=i['key'], action=i['action'], toggle=toggle)
                 self.playerbox.addWidget(self.btn[label])
             x+=1
 
     def mediaInfo(self, f):
-        title=f
+        title=os.path.basename(f)
         length=0
         bitrate=0
         quality=0
         channels=1
         info={'title':title, 'length':length, 'bitrate':bitrate, 'quality':quality, 'channels':channels}
         self.playListInfo[f]=info
         return info
@@ -234,23 +255,23 @@
             self.infoBox.feed(self.script)
             pass
         elif self.mode=='play':
             self.infoBox.feed(self.t.clear())
             self.infoBox.feed(self.t.ansicolor(27))
             title=""
             title=f'{self.playlist.index(self.filename)+1}. '
-            if self.playListInfo[self.filename]: 
+            if self.playListInfo[self.filename]:
                 title+=self.playListInfo[self.filename]['title']
                 title+=f' ({minsec(self.playListInfo[self.filename]["length"])})'
             self.infoBox.feed(self.t.gotoxy(1, 1))
-            self.infoBox.feed(title)
+            self.infoBox.feed(scroll_string(title, 38, clock=t))
             quality=0
             bitrate=0
             channels=0
-            if self.playListInfo[self.filename]: 
+            if self.playListInfo[self.filename]:
                 quality=int(self.playListInfo[self.filename]["quality"])
                 bitrate=int(self.playListInfo[self.filename]["bitrate"])
                 channels=int(self.playListInfo[self.filename]["channels"])
             self.infoBox.feed(self.t.gotoxy(1, 3))
             self.infoBox.feed(f'{int(quality)}kbps')
             self.infoBox.feed(self.t.gotoxy(14, 3))
             self.infoBox.feed(f'{bitrate}kHz')
@@ -289,55 +310,66 @@
         self.timeBox.feed(self.t.gotoxy(1, 4))
         self.timeBox.feed(self.t.ansicolor(rcolor, 233, bold=True))
         self.timeBox.feed(i['label'])
         i=self.icons['shuffle']
         self.timeBox.feed(self.t.gotoxy(1, 5))
         self.timeBox.feed(self.t.ansicolor(scolor, 233, bold=True))
         self.timeBox.feed(i['label'])
-        buffer+=self.playerbox.draw()
+        playerbuffer=self.playerbox.draw()
+        if playerbuffer!=self.playerbuffer:
+            buffer+=playerbuffer
+            self.playerbuffer=playerbuffer
         if self.showPlayList:
             self.playlistbox.feed(f'{self.t.clear()}')
             startline=self.playlist.index(self.filename)
-            if startline+self.h-3>len(self.playlist):
-                startline=len(self.playlist)-(self.h-2)
+            if startline+self.playlistbox.h-3>len(self.playlist):
+                startline=len(self.playlist)-(self.playlistbox.h-2)
             if startline<0:
                 startline=0
-            for n in range(self.h-2):
+            for n in range(self.playlistbox.h-2):
                 color=27
                 if n+startline<len(self.playlist):
                     f=self.playlist[startline+n]
                     if f==self.filename:
                         color=46
                     self.playlistbox.feed(f'{self.t.gotoxy(1,n+1)}')
                     self.playlistbox.feed(f'{self.t.ansicolor(color)}')
                     title=f
                     tm="00:00"
                     if self.playListInfo[f]:
                         title=f"{self.playListInfo[f]['title']}"
                         tm=f"{minsec(self.playListInfo[f]['length'])}"
-                    self.playlistbox.feed(f'{n+startline+1}. {title}')
-                    self.playlistbox.feed(f'{self.t.gotoxy(self.w-3-len(tm),n+1)}')
+                    else:
+                        title=os.path.basename(title)
+                    PL_line_length=self.playlistbox.w-4-len(f' {tm}')-len(f'{n+startline+1}. ')
+                    self.playlistbox.feed(f'{n+startline+1}. {scroll_string(title, PL_line_length, clock=0)}')
+                    self.playlistbox.feed(f'{self.t.gotoxy(self.playlistbox.w-3-len(tm), n+1)}')
                     self.playlistbox.feed(f'{tm}')
                 else:
-                    self.playlistbox.feed(f'{self.t.gotoxy(1,n+1)} ') 
-            buffer+=self.playlistbox.draw()
+                    self.playlistbox.feed(f'{self.t.gotoxy(1,n+1)} ')
+
+            playlistbuffer=self.playlistbox.draw()
+            if playlistbuffer!=self.playlistbuffer:
+                buffer+=playlistbuffer
+                self.playlistbuffer=playlistbuffer
         else:
             if self.clearPlayList:
                 self.clearPlayList=False
                 buffer+=self.t.reset()
-                for y in range(self.y+self.h,self.y+2*self.h):
+                for y in range(self.y+self.h,self.y+self.h+self.playlistbox.h):
                     buffer+=self.t.gotoxy(self.x, y)
                     for x in range(0, self.w):
                         buffer+=' '
         #print(self.anim[self.frame % len(self.anim)])
         self.frame +=1
         return buffer
 
     def togglePlayList(self):
         self.showPlayList=not self.showPlayList
+        self.playlistbuffer=''
         if not self.showPlayList:
             self.clearPlayList=True
 
     def load(self, filename):
         info=self.player.load(filename)
         self.playListInfo[filename]=info
         self.filename=filename
@@ -347,32 +379,38 @@
 
     def quit(self):
         if self.mode=='record':
             #TODO save prompt
             if(1):
                 self.save(self.filename)
         self.stop()
-        quit()
+        if self.go:
+            self.go=False
+        else:
+            pass
+            #quit()
 
     def next(self):
         i=self.playlist.index(self.filename)
         i+=1
         if i>=len(self.playlist):
             i=0
+        p=self.player.au.status
         self.load(self.playlist[i])
-        if self.mode=='play':
+        if p==PLAY:
             self.play()
 
     def prev(self):
         i=self.playlist.index(self.filename)
         i-=1
         if i<0:
             i=len(self.playlist)-1
+        p=self.player.au.status
         self.load(self.playlist[i])
-        if self.mode=='play':
+        if p==PLAY:
             self.play()
 
     def endHandler(self):
         if self.player.au.status==PLAY:
             if self.mode=='play':
                 if self.repeat:
                     self.stop()
@@ -422,29 +460,46 @@
         self.player.denoise()
 
     def normalize(self):
         self.player.normalize()
 
 def main():
     parser=OptionParser(usage="usage: %prog [options] AUDIO_FILES")
-    parser.add_option("-r", "--record", action='store_true', dest="record", 
+    parser.add_option("-p", "--play", action='store_true', dest="play",
+            default=False, help="Play immediately.")
+    parser.add_option("-r", "--record", action='store_true', dest="record",
             default=False, help="Record mode.")
+    parser.add_option("-S", "--shuffle", action='store_true', dest="shuffle",
+            default=False, help="Turn on shuffle.")
+    parser.add_option("-R", "--repeat", action='store_true', dest="repeat",
+            default=False, help="Turn on repeat.")
+    parser.add_option("-L", "--list", action='store_true', dest="playlist",
+            default=False, help="show playlist.")
     parser.add_option("-v", "--verbose", dest="debug", default="info",
             help="Show debug messages.[debug, info, warning]")
     parser.add_option("-s", dest="script", default="No script was given.",
             help="Script for record mode.")
-    parser.add_option("-x", dest="x", default=1, help="Top left coordinate.")
-    parser.add_option("-y", dest="y", default=1, help="Top left coordinate.")
-
+    parser.add_option("-x", dest="x", default=1, help="Left coordinate.")
+    parser.add_option("-y", dest="y", default=1, help="Top coordinate.")
     (options, args)=parser.parse_args()
     if len(args)==0:
         parser.print_help()
         return
     mode='play'
     if options.record:
         mode='record'
-    tp=termplayer(x=int(options.x), y=int(options.y), mode=mode, script=options.script, files=args)
+    tp=termplayer(x=int(options.x), y=int(options.y), mode=mode,
+                  script=options.script, files=args,
+                  shuffle=options.shuffle, repeat=options.repeat,
+                  play=options.play,
+                  playlist=options.playlist and not options.record)
+    tp.kb.disable_keyboard_echo()
+    print(tp.t.disable_cursor(), end='')
+    print(tp.t.disable_mouse(), end='')
     tp.guiLoop()
+    tp.kb.enable_keyboard_echo()
+    print(tp.t.enable_cursor(), end='')
+    print(tp.t.enable_mouse(), end='')
     return
 
 if __name__ == "__main__":
     main()
```

### Comparing `gm_pymms-0.0.2/gm_pymms.egg-info/PKG-INFO` & `gm_pymms-0.0.3/gm_pymms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gm-pymms
-Version: 0.0.2
+Version: 0.0.3
 Summary: python xmms inspired media player/recorder
 Home-page: https://github.com/gretchycat/pymms
 Author: Gretchen Maculo
 Author-email: gretchen.maculo@gmail.com
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gm_pymms-0.0.2/setup.cfg` & `gm_pymms-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gm_pymms
-version = 0.0.2
+version = 0.0.3
 url = https://github.com/gretchycat/pymms
 author = Gretchen Maculo
 author_email = gretchen.maculo@gmail.com
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
```

### Comparing `gm_pymms-0.0.2/setup.py` & `gm_pymms-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 shutil.copyfile('gm_pymms/termplayer.py', 'gm_pymms/pymms')
 
 setup(
     name='gm_pymms',
-    version='0.0.2',
+    version='0.0.3',
     license='GPL3',
     url='https://github.com/gretchycat/pymms',
     author='Gretchen Maculo',
     author_email='gretchen.maculo@gmail.com',
     description='python xmms inspired media player/recorder',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

