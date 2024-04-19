# Comparing `tmp/bosing-1.0.0b4.tar.gz` & `tmp/bosing-1.0.1.tar.gz`

## Comparing `bosing-1.0.0b4.tar` & `bosing-1.0.1.tar`

### file list

```diff
@@ -1,129 +1,131 @@
--rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.editorconfig
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.gitattributes
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.readthedocs.yaml
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.0b4/Bosing.sln
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.0b4/Directory.Build.props
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b4/VERSION.txt
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.0b4/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.0b4/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b4/exclusion.dic
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.github/dependabot.yml
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/Program.cs
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/_native.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/_utils.py
--rw-r--r--   0        0        0    18568 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/models.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/Makefile
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/api.rst
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/conf.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/index.rst
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/instruction.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/make.bat
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/quickstart.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/requirements.txt
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/schedule.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/example/schedule.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/example/schedule_stress.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/tests/test_basic.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BiquadChain.cs
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BiquadCoefficients.cs
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BiquadFilter.cs
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Bosing.csproj
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BosingOptions.cs
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/ComplexReadOnlySpan.cs
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/ComplexSpan.cs
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Envelope.cs
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/EnvelopeCacheKey.cs
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/EnvelopeInfo.cs
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/EnvelopeSample.cs
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/FirCoefficients.cs
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/HannPulseShape.cs
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/IPulseShape.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/InterpolatedPulseShape.cs
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/IqPair.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/MathUtils.cs
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PhaseTrackingTransform.cs
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PooledComplexArray.cs
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PostProcessTransform.cs
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PulseList.cs
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/SignalFilter.cs
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/TimeAxisUtils.cs
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/TrianglePulseShape.cs
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/ValueArray.cs
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/WaveformSampler.cs
--rw-r--r--   0        0        0    30123 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/WaveformUtils.cs
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/AbsoluteSchedule.cs
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/Alignment.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ArrangeOption.cs
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/BarrierElement.cs
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/GridLength.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/GridLengthUnit.cs
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/GridSchedule.cs
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/PlayElement.cs
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/RepeatElement.cs
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/Schedule.cs
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ScheduleElement.cs
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/SetFrequencyElement.cs
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/SetPhaseElement.cs
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ShiftFrequencyElement.cs
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ShiftPhaseElement.cs
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/StackSchedule.cs
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/SwapPhaseElement.cs
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/Thickness.cs
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Api.cs
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Bosing.Aot.csproj
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/ScheduleRunner.cs
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/UnsafeMemoryManager.cs
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/BarrierElementDto.cs
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/BiquadDto.cs
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ChannelInfo.cs
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/GridScheduleDto.cs
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/HannShapeInfo.cs
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/IqCalibration.cs
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/OptionsDto.cs
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/PlayElementDto.cs
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/RepeatElementDto.cs
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ScheduleElementDto.cs
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ScheduleRequest.cs
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/SetPhaseElementDto.cs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ShapeInfo.cs
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/StackScheduleDto.cs
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Bosing.Tests.csproj
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/EnvelopeInfoTests.cs
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/HannPulseShapeTests.cs
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/IntegrationTests.cs
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/IqPairTests.cs
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/MathUtilsTests.cs
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/PooledComplexArrayTests.cs
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/PulseListTests.cs
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/TimeAxisUtilsTests.cs
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/ToleranceComparer.cs
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/TrianglePulseShapeTests.cs
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Usings.cs
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/WaveformUtilsTests.cs
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleTests.cs
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.0b4/LICENSE.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bosing-1.0.0b4/README.md
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 bosing-1.0.0b4/hatch_build.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bosing-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 bosing-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.1/.editorconfig
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.1/.gitattributes
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 bosing-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.1/Bosing.sln
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.1/Directory.Build.props
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bosing-1.0.1/VERSION.txt
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.1/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.1/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.1/exclusion.dic
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 bosing-1.0.1/ruff_defaults.toml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 bosing-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/Program.cs
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/__init__.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/_native.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/_utils.py
+-rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/models.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/Makefile
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/api.rst
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/conf.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/index.rst
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/instruction.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/make.bat
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/quickstart.rst
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/requirements.txt
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/schedule.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bosing-1.0.1/python/example/schedule.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bosing-1.0.1/python/example/schedule_stress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bosing-1.0.1/python/tests/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bosing-1.0.1/python/tests/test_basic.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BiquadChain.cs
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BiquadCoefficients.cs
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BiquadFilter.cs
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Bosing.csproj
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BosingOptions.cs
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/ComplexReadOnlySpan.cs
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/ComplexSpan.cs
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Envelope.cs
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/EnvelopeCacheKey.cs
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/EnvelopeInfo.cs
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/EnvelopeSample.cs
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/FirCoefficients.cs
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/HannPulseShape.cs
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/IPulseShape.cs
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/InterpolatedPulseShape.cs
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/IqPair.cs
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/MathUtils.cs
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PhaseTrackingTransform.cs
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PooledComplexArray.cs
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PostProcessTransform.cs
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PulseList.cs
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/SignalFilter.cs
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/TimeAxisUtils.cs
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/TrianglePulseShape.cs
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/ValueArray.cs
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/WaveformSampler.cs
+-rw-r--r--   0        0        0    30212 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/WaveformUtils.cs
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/AbsoluteSchedule.cs
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/Alignment.cs
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ArrangeOption.cs
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/BarrierElement.cs
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/GridLength.cs
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/GridLengthUnit.cs
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/GridSchedule.cs
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/PlayElement.cs
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/RepeatElement.cs
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/Schedule.cs
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ScheduleElement.cs
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/SetFrequencyElement.cs
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/SetPhaseElement.cs
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ShiftFrequencyElement.cs
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ShiftPhaseElement.cs
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/StackSchedule.cs
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/SwapPhaseElement.cs
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/Thickness.cs
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Api.cs
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Bosing.Aot.csproj
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/ScheduleRunner.cs
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/UnsafeMemoryManager.cs
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/BarrierElementDto.cs
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/BiquadDto.cs
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ChannelInfo.cs
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/GridScheduleDto.cs
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/HannShapeInfo.cs
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/IqCalibration.cs
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/OptionsDto.cs
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/PlayElementDto.cs
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/RepeatElementDto.cs
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ScheduleElementDto.cs
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ScheduleRequest.cs
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/SetPhaseElementDto.cs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ShapeInfo.cs
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/StackScheduleDto.cs
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Bosing.Tests.csproj
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/EnvelopeInfoTests.cs
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/HannPulseShapeTests.cs
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/IntegrationTests.cs
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/IqPairTests.cs
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/MathUtilsTests.cs
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/PooledComplexArrayTests.cs
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/PulseListTests.cs
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/TimeAxisUtilsTests.cs
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/ToleranceComparer.cs
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/TrianglePulseShapeTests.cs
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Usings.cs
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/WaveformUtilsTests.cs
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/ScheduleTests.cs
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bosing-1.0.1/README.md
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 bosing-1.0.1/hatch_build.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bosing-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bosing-1.0.1/PKG-INFO
```

### Comparing `bosing-1.0.0b4/.editorconfig` & `bosing-1.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/.gitattributes` & `bosing-1.0.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/.readthedocs.yaml` & `bosing-1.0.1/.readthedocs.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
   os: ubuntu-22.04
   tools:
     python: "3.12"
     # You can also specify other tool versions:
     # nodejs: "20"
     # rust: "1.70"
     # golang: "1.20"
+  apt_packages:
+    - dotnet-sdk-8.0
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
   configuration: python/docs/conf.py
   # You can configure Sphinx to use a different builder, for instance use the dirhtml builder for simpler URLs
   # builder: "dirhtml"
   # Fail on all warnings to avoid broken references
```

### Comparing `bosing-1.0.0b4/Bosing.sln` & `bosing-1.0.1/Bosing.sln`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md` & `bosing-1.0.1/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/WaveGenBenchmarks.WaveformUtilsBench-report-github.md` & `bosing-1.0.1/WaveGenBenchmarks.WaveformUtilsBench-report-github.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/.github/workflows/ci.yml` & `bosing-1.0.1/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
       - beta
   pull_request:
     branches:
       - main
       - alpha
       - beta
 
-concurrency: 
+concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
-permissions: 
+permissions:
   contents: read
 
 jobs:
   # Should run on every push and PR
   test:
     name: Test
     runs-on: ubuntu-latest
@@ -42,15 +42,15 @@
       - name: Test
         run: dotnet test --no-build --verbosity normal
       - name: Install hatch
         run: |
           python -m pip install --upgrade pip
           pip install hatch
       - name: Test
-        run: hatch run test:run 
+        run: hatch run test:run
 
   # Should run on every push and PR, but only run semantic-release on push
   release:
     name: Run semantic-release
     runs-on: ubuntu-latest
     needs: test
     permissions:
@@ -193,15 +193,15 @@
       - build-wheel
       - build-wheel-linux
       - sdist
       - release
     if: needs.release.outputs.published == 'true' && github.event_name == 'push'
     runs-on: ubuntu-latest
     environment: pypi
-    permissions: 
+    permissions:
       id-token: write
     steps:
       - name: Download artifacts
         uses: actions/download-artifact@v4
         with:
           path: dist
           merge-multiple: true
```

### Comparing `bosing-1.0.0b4/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs` & `bosing-1.0.1/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/examples/WaveGenBenchmarks/WaveformUtilsBench.cs` & `bosing-1.0.1/examples/WaveGenBenchmarks/WaveformUtilsBench.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/bosing/__init__.py` & `bosing-1.0.1/python/bosing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 .. caution::
 
     All phase values are in number of cycles. For example, a phase of
     :math:`0.25` means :math:`\\pi/2` radians.
 """
 
-from ._utils import generate_waveforms
-from .models import (
+from bosing._utils import generate_waveforms
+from bosing.models import (
     Absolute,
-    AbsoluteEntry,
+    AbsoluteEntry,  # noqa: F401
     Alignment,
     Barrier,
     Biquad,
     Channel,
-    Element,
+    Element,  # noqa: F401
     Grid,
-    GridEntry,
-    GridLength,
+    GridEntry,  # noqa: F401
+    GridLength,  # noqa: F401
     Hann,
     Interp,
     IqCali,
     Options,
     Play,
     Repeat,
     SetFreq,
```

### Comparing `bosing-1.0.0b4/python/bosing/_native.py` & `bosing-1.0.1/python/bosing/_native.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from __future__ import annotations
+
 import ctypes
 import sys
-import typing
 from enum import Enum
 from pathlib import Path
 
 import numpy as np
 
 if sys.platform == "win32":
     lib_path = Path(__file__).parent / "lib" / "Bosing.Aot.dll"
 elif sys.platform == "linux":
     lib_path = Path(__file__).parent / "lib" / "Bosing.Aot.so"
 elif sys.platform == "darwin":
     lib_path = Path(__file__).parent / "lib" / "Bosing.Aot.dylib"
 else:
-    raise Exception(f"Unsupported platform: {sys.platform}")
+    msg = f"Unsupported platform: {sys.platform}"
+    raise RuntimeError(msg)
 
 lib = ctypes.cdll.LoadLibrary(str(lib_path.resolve()))
 
 
 # enum ErrorCode
 # {
 #     Success = 0,
@@ -44,20 +46,21 @@
     ctypes.c_char_p,
     ctypes.c_int,
     ctypes.POINTER(ctypes.c_void_p),
 ]
 Bosing_Run.restype = ctypes.c_int
 
 
-def run(msg: bytes) -> ctypes.c_void_p:
+def run(req_msg: bytes) -> ctypes.c_void_p:
     handle = ctypes.c_void_p()
-    ret = Bosing_Run(msg, len(msg), ctypes.byref(handle))
+    ret = Bosing_Run(req_msg, len(req_msg), ctypes.byref(handle))
     if ret != 0:
         err = ErrorCode(ret)
-        raise Exception(f"Failed to run Bosing, error code: {err}")
+        msg = f"Failed to run Bosing, error code: {err}"
+        raise RuntimeError(msg)
     return handle
 
 
 # int Bosing_CopyWaveform(void* handle, char* name, float* i, float* q, int length)
 Bosing_CopyWaveform = lib.Bosing_CopyWaveform
 Bosing_CopyWaveform.argtypes = [
     ctypes.c_void_p,
@@ -65,33 +68,33 @@
     ctypes.POINTER(ctypes.c_float),
     ctypes.POINTER(ctypes.c_float),
     ctypes.c_int,
 ]
 Bosing_CopyWaveform.restype = ctypes.c_int
 
 
-def copy_waveform(
-    handle: ctypes.c_void_p, name: str, length: int
-) -> typing.Tuple[np.ndarray, np.ndarray]:
+def copy_waveform(handle: ctypes.c_void_p, name: str, length: int) -> tuple[np.ndarray, np.ndarray]:
     wave_i = np.empty(length, dtype=np.float32)
     wave_q = np.empty(length, dtype=np.float32)
     pstr = name.encode("utf-8")
     ptr_i_float = wave_i.ctypes.data_as(ctypes.POINTER(ctypes.c_float))
     ptr_q_float = wave_q.ctypes.data_as(ctypes.POINTER(ctypes.c_float))
     ret = Bosing_CopyWaveform(handle, pstr, ptr_i_float, ptr_q_float, length)
     if ret != 0:
         err = ErrorCode(ret)
-        raise Exception(f"Failed to copy waveform, error code: {err}")
+        msg = f"Failed to copy waveform, error code: {err}"
+        raise RuntimeError(msg)
     return wave_i, wave_q
 
 
 # int Bosing_FreeWaveform(void* handle)
 Bosing_FreeWaveform = lib.Bosing_FreeWaveform
 Bosing_FreeWaveform.argtypes = [ctypes.c_void_p]
 Bosing_FreeWaveform.restype = ctypes.c_int
 
 
 def free_waveform(handle: ctypes.c_void_p) -> None:
     ret = Bosing_FreeWaveform(handle)
     if ret != 0:
         err = ErrorCode(ret)
-        raise Exception(f"Failed to free waveform, error code: {err}")
+        msg = f"Failed to free waveform, error code: {err}"
+        raise RuntimeError(msg)
```

### Comparing `bosing-1.0.0b4/python/bosing/_utils.py` & `bosing-1.0.1/python/bosing/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-import typing
+from __future__ import annotations
 
-import numpy as np
+from collections.abc import Iterable  # noqa: TCH003
 
-from ._native import copy_waveform, free_waveform, run
-from .models import Channel, Element, Options, Request, Shape
+import numpy as np  # noqa: TCH002
+
+from bosing._native import copy_waveform, free_waveform, run
+from bosing.models import Channel, Element, Options, Request, Shape
 
 
 def generate_waveforms(
-    channels: typing.Iterable[Channel],
-    shapes: typing.Iterable[Shape],
+    channels: Iterable[Channel],
+    shapes: Iterable[Shape],
     schedule: Element,
-    options: typing.Optional[Options] = None,
-) -> typing.Dict[str, typing.Tuple[np.ndarray, np.ndarray]]:
+    options: Options | None = None,
+) -> dict[str, tuple[np.ndarray, np.ndarray]]:
     """Generate waveforms.
 
     :param channels: Information about the channels used in the schedule.
     :param shapes: Information about the shapes used in the schedule.
     :param schedule: The root element of the schedule.
     :param options: Various options for the waveform generation.
     :return: A dictionary of waveforms, where the key is the channel name and
         the value is a tuple of two numpy arrays representing the I and Q
         components of the waveform.
+    :raises RuntimeError: If the waveform generation fails.
     """
     request = Request(
         channels=channels,
         shapes=shapes,
         schedule=schedule,
         options=options or Options(),
     )
```

### Comparing `bosing-1.0.0b4/python/bosing/models.py` & `bosing-1.0.1/python/bosing/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Data models for the Bosing service."""
 
+from __future__ import annotations
+
 import enum as _enum
 import math as _math
 import typing as _typing
+from typing import ClassVar
 
 import attrs as _attrs
 import msgpack as _msgpack
 
 
 @_attrs.frozen
 class MsgObject:
@@ -21,32 +24,33 @@
     def data(self) -> tuple:
         """The data of the message object to be serialized."""
         return _attrs.astuple(self, recurse=False)
 
     def packb(self) -> bytes:
         """Serialize the message object to bytes in msgpack format."""
 
-        def encode(obj: _typing.Union[MsgObject, _enum.Enum]):
+        def encode(obj: MsgObject | _enum.Enum):
             if isinstance(obj, MsgObject):
                 return obj.data
             if isinstance(obj, _enum.Enum):
                 return obj.value
-            raise TypeError(f"Cannot encode object of type {type(obj)}")
+            msg = f"Cannot encode object of type {type(obj)}"
+            raise TypeError(msg)
 
         return _msgpack.packb(self, default=encode)  # type: ignore
 
 
 @_attrs.frozen
 class UnionObject(MsgObject):
     """Base class for all union objects.
 
     A union object is a message object that can be one of several types.
     """
 
-    TYPE_ID: _typing.ClassVar[int]
+    TYPE_ID: ClassVar[int]
 
     @property
     def data(self) -> tuple:
         return (self.TYPE_ID, super().data)
 
 
 @_attrs.frozen
@@ -100,17 +104,17 @@
 
     name: str
     base_freq: float
     sample_rate: float
     length: int
     delay: float = 0
     align_level: int = -10
-    iq_calibration: _typing.Optional[IqCali] = None
-    iir: _typing.List[Biquad] = _attrs.field(factory=list, converter=list)
-    fir: _typing.List[float] = _attrs.field(factory=list, converter=list)
+    iq_calibration: IqCali | None = None
+    iir: list[Biquad] = _attrs.field(factory=list, converter=list)
+    fir: list[float] = _attrs.field(factory=list, converter=list)
 
 
 @_attrs.frozen
 class Options(MsgObject):
     """Various options for waveform generation.
 
     :param time_tolerance: The time tolerance of the scheduler.
@@ -131,26 +135,22 @@
     END = 0
     START = 1
     CENTER = 2
     STRETCH = 3
     """Stretch to fill parent element."""
 
 
-def _convert_margin(
-    margin: _typing.Union[float, _typing.Tuple[float, float]]
-) -> _typing.Tuple[float, float]:
+def _convert_margin(margin: float | tuple[float, float]) -> tuple[float, float]:
     if not isinstance(margin, tuple):
         margin = (margin, margin)
     return margin
 
 
 def _convert_alignment(
-    alignment: _typing.Union[
-        _typing.Literal["end", "start", "center", "stretch"], Alignment
-    ]
+    alignment: _typing.Literal["end", "start", "center", "stretch"] | Alignment,
 ) -> Alignment:
     if isinstance(alignment, str):
         return Alignment[alignment.upper()]
     return alignment
 
 
 @_attrs.frozen
@@ -167,16 +167,16 @@
 
 @_attrs.frozen
 class Interp(Shape):
     """An interpolated shape."""
 
     TYPE_ID = 1
 
-    x_array: _typing.List[float] = _attrs.field(converter=list)
-    y_array: _typing.List[float] = _attrs.field(converter=list)
+    x_array: list[float] = _attrs.field(converter=list)
+    y_array: list[float] = _attrs.field(converter=list)
 
 
 @_attrs.frozen
 class Element(UnionObject):
     """Base class for schedule elements.
 
     A schedule element is a node in the tree structure of a schedule similar to
@@ -200,22 +200,18 @@
     :param duration: Requested duration of the element. If ``None``, the actual
         duration is determined by the measuring and arranging process. Default
         to ``None``.
     :param max_duration: Maximum duration of the element. Default to infinity.
     :param min_duration: Minimum duration of the element. Default to 0.
     """
 
-    margin: _typing.Tuple[float, float] = _attrs.field(
-        kw_only=True, default=(0, 0), converter=_convert_margin
-    )
-    alignment: Alignment = _attrs.field(
-        kw_only=True, default=Alignment.END, converter=_convert_alignment
-    )
+    margin: tuple[float, float] = _attrs.field(kw_only=True, default=(0, 0), converter=_convert_margin)
+    alignment: Alignment = _attrs.field(kw_only=True, default=Alignment.END, converter=_convert_alignment)
     visibility: bool = _attrs.field(kw_only=True, default=True)
-    duration: _typing.Optional[float] = _attrs.field(kw_only=True, default=None)
+    duration: float | None = _attrs.field(kw_only=True, default=None)
     max_duration: float = _attrs.field(kw_only=True, default=_math.inf)
     min_duration: float = _attrs.field(kw_only=True, default=0)
 
 
 @_attrs.frozen
 class Play(Element):
     """A pulse play element.
@@ -358,15 +354,15 @@
     all channels in its parent element.
 
     :param channel_ids: Target channel IDs. Default to empty.
     """
 
     TYPE_ID = 6
 
-    channel_ids: _typing.List[int] = _attrs.field(converter=list, factory=list)
+    channel_ids: list[int] = _attrs.field(converter=list, factory=list)
 
 
 @_attrs.frozen
 class Repeat(Element):
     """A repeated schedule element.
 
     :param child: The repeated element.
@@ -387,15 +383,15 @@
     BACKWARDS = 0
     """Arrange from the end of the schedule."""
     FORWARDS = 1
     """Arrange from the start of the schedule."""
 
 
 def _convert_direction(
-    direction: _typing.Union[_typing.Literal["backwards", "forwards"], ArrangeDirection]
+    direction: _typing.Literal["backwards", "forwards"] | ArrangeDirection,
 ) -> ArrangeDirection:
     if isinstance(direction, str):
         return ArrangeDirection[direction.upper()]
     return direction
 
 
 @_attrs.frozen
@@ -410,20 +406,20 @@
 
     :param children: Child elements.
     :param direction: The direction of arrangement.
     """
 
     TYPE_ID = 8
 
-    children: _typing.List[Element] = _attrs.field(converter=list, factory=list)
+    children: list[Element] = _attrs.field(converter=list, factory=list)
     direction: ArrangeDirection = _attrs.field(
         kw_only=True, default=ArrangeDirection.BACKWARDS, converter=_convert_direction
     )
 
-    def with_children(self, *children: Element) -> "Stack":
+    def with_children(self, *children: Element) -> Stack:
         """Create a new stack with different children.
 
         :param children: The new children.
         :return: The new stack.
         """
         return _attrs.evolve(self, children=children)
 
@@ -436,34 +432,30 @@
     :param element: The child element.
     """
 
     time: float
     element: Element
 
     @classmethod
-    def from_tuple(
-        cls, obj: _typing.Union[Element, _typing.Tuple[float, Element], "AbsoluteEntry"]
-    ) -> "AbsoluteEntry":
+    def from_tuple(cls, obj: Element | tuple[float, Element] | AbsoluteEntry) -> AbsoluteEntry:
         """Create an absolute entry from a tuple.
 
         :param obj: The object to be converted.
         :return: The converted object.
         """
         if isinstance(obj, Element):
             return cls(time=0, element=obj)
         if isinstance(obj, tuple):
             return cls(time=obj[0], element=obj[1])
         return obj
 
 
 def _convert_abs_entries(
-    entries: _typing.List[
-        _typing.Union[Element, _typing.Tuple[float, Element], AbsoluteEntry]
-    ]
-) -> _typing.List[AbsoluteEntry]:
+    entries: list[Element | tuple[float, Element] | AbsoluteEntry],
+) -> list[AbsoluteEntry]:
     return [AbsoluteEntry.from_tuple(obj) for obj in entries]
 
 
 @_attrs.frozen
 class Absolute(Element):
     """An absolute schedule element.
 
@@ -475,21 +467,17 @@
         can be either an :class:`Element` or ``(time, element)``. Default
         ``time`` is 0.
     :type children: list[Element | tuple[float, Element] | AbsoluteEntry]
     """
 
     TYPE_ID = 9
 
-    children: _typing.List[AbsoluteEntry] = _attrs.field(
-        converter=_convert_abs_entries, factory=list
-    )
+    children: list[AbsoluteEntry] = _attrs.field(converter=_convert_abs_entries, factory=list)
 
-    def with_children(
-        self, *children: _typing.Union[Element, _typing.Tuple[float, Element]]
-    ) -> "Absolute":
+    def with_children(self, *children: Element | tuple[float, Element]) -> Absolute:
         """Create a new absolute schedule with different children.
 
         :param children: The new children.
         :return: The new absolute schedule.
         """
         return _attrs.evolve(self, children=children)
 
@@ -514,30 +502,30 @@
     or automatically.
     """
 
     value: float
     unit: GridLengthUnit
 
     @classmethod
-    def auto(cls) -> "GridLength":
+    def auto(cls) -> GridLength:
         """Create an automatic grid length."""
         return cls(value=_math.nan, unit=GridLengthUnit.AUTO)
 
     @classmethod
-    def star(cls, value: float) -> "GridLength":
+    def star(cls, value: float) -> GridLength:
         """Create a star grid length."""
         return cls(value=value, unit=GridLengthUnit.STAR)
 
     @classmethod
-    def abs(cls, value: float) -> "GridLength":
-        """Create an absolute grid length."""
+    def fixed(cls, value: float) -> GridLength:
+        """Create an fixed grid length."""
         return cls(value=value, unit=GridLengthUnit.SECOND)
 
     @classmethod
-    def parse(cls, value: _typing.Union[str, float]) -> "GridLength":
+    def parse(cls, value: str | float) -> GridLength:
         """Create a grid length from a string or a float.
 
         The value can be one of the following formats:
 
         ``"10e-9"`` or 10e-9
             10 nanoseconds
 
@@ -549,73 +537,56 @@
 
         ``"auto"``
             Automatic
 
         :param value: The value to parse.
         """
         if isinstance(value, (float, int)):
-            return cls.abs(value)
+            return cls.fixed(value)
         if value.lower() == "auto":
             return cls.auto()
         if value.endswith("*"):
             return cls.star(float(value[:-1]))
-        return cls.abs(float(value))
+        return cls.fixed(float(value))
 
 
 @_attrs.frozen
 class GridEntry(MsgObject):
     """An entry in the grid schedule."""
 
     column: int
     span: int
     element: Element
 
     @classmethod
     def from_tuple(
         cls,
-        obj: _typing.Union[
-            Element,
-            _typing.Tuple[int, Element],
-            _typing.Tuple[int, int, Element],
-            "GridEntry",
-        ],
-    ) -> "GridEntry":
+        obj: Element | tuple[int, Element] | tuple[int, int, Element] | GridEntry,
+    ) -> GridEntry:
         """Create a grid entry from a tuple.
 
         :param obj: The tuple to convert.
         """
         if isinstance(obj, Element):
             return cls(column=0, span=1, element=obj)
         if isinstance(obj, tuple):
-            if len(obj) == 2:
+            if len(obj) == 2:  # noqa: PLR2004
                 return cls(column=obj[0], span=1, element=obj[1])
             return cls(column=obj[0], span=obj[1], element=obj[2])
         return obj
 
 
 def _convert_grid_entries(
-    entries: _typing.List[
-        _typing.Union[
-            Element,
-            _typing.Tuple[int, Element],
-            _typing.Tuple[int, int, Element],
-            GridEntry,
-        ]
-    ]
-) -> _typing.List[GridEntry]:
+    entries: list[Element | tuple[int, Element] | tuple[int, int, Element] | GridEntry],
+) -> list[GridEntry]:
     return [GridEntry.from_tuple(obj) for obj in entries]
 
 
-def _convert_columns(
-    columns: _typing.List[_typing.Union[GridLength, str, float]]
-) -> _typing.List[GridLength]:
-    return [
-        GridLength.parse(column) if not isinstance(column, GridLength) else column
-        for column in columns
-    ]
+def _convert_columns(columns: list[GridLength | str | float]) -> list[GridLength]:
+    return [GridLength.parse(column) if not isinstance(column, GridLength) else column for column in columns]
 
 
 @_attrs.frozen
 class Grid(Element):
     """A grid schedule element.
 
     :param children: Child elements with column index and span. Each item in the
@@ -627,31 +598,23 @@
         be specified as a :class:`GridLength`, a string, or a float. See
         :meth:`GridLength.parse` for details.
     :type columns: list[GridLength | str | float]
     """
 
     TYPE_ID = 10
 
-    children: _typing.List[GridEntry] = _attrs.field(
-        converter=_convert_grid_entries, factory=list
-    )
+    children: list[GridEntry] = _attrs.field(converter=_convert_grid_entries, factory=list)
     """Child elements with grid positioning."""
-    columns: _typing.List[GridLength] = _attrs.field(
-        converter=_convert_columns, factory=list
-    )
+    columns: list[GridLength] = _attrs.field(converter=_convert_columns, factory=list)
     """Definitions of grid columns."""
 
     def with_children(
         self,
-        *children: _typing.Union[
-            Element,
-            _typing.Tuple[int, Element],
-            _typing.Tuple[int, int, Element],
-        ],
-    ) -> "Grid":
+        *children: Element | tuple[int, Element] | tuple[int, int, Element],
+    ) -> Grid:
         """Create a new grid schedule with different children.
 
         :param children: The new children.
         :return: The new grid schedule.
         """
         return _attrs.evolve(self, children=children)
 
@@ -662,11 +625,11 @@
 
     :param channels: Information about the channels used in the schedule.
     :param shapes: Information about the shapes used in the schedule.
     :param schedule: The root element of the schedule.
     :param options: Various options for waveform generation.
     """
 
-    channels: _typing.List[Channel] = _attrs.field(converter=list)
-    shapes: _typing.List[Shape] = _attrs.field(converter=list)
+    channels: list[Channel] = _attrs.field(converter=list)
+    shapes: list[Shape] = _attrs.field(converter=list)
     schedule: Element
     options: Options = _attrs.field(factory=Options)
```

### Comparing `bosing-1.0.0b4/python/docs/Makefile` & `bosing-1.0.1/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/docs/conf.py` & `bosing-1.0.1/python/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.viewcode",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.intersphinx",
+    "matplotlib.sphinxext.plot_directive",
 ]
 
 autodoc_typehints = "description"
-autodoc_mock_imports = ["bosing._native"]
 autosummary_imported_members = True
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
 }
 
 templates_path = ["_templates"]
```

### Comparing `bosing-1.0.0b4/python/docs/instruction.rst` & `bosing-1.0.1/python/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/docs/make.bat` & `bosing-1.0.1/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/docs/schedule.rst` & `bosing-1.0.1/python/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/docs/_templates/autosummary/module.rst` & `bosing-1.0.1/python/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/example/schedule.py` & `bosing-1.0.1/python/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/example/schedule_stress.py` & `bosing-1.0.1/python/example/schedule_stress.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/python/tests/test_basic.py` & `bosing-1.0.1/python/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/BiquadChain.cs` & `bosing-1.0.1/src/Bosing/BiquadChain.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/BiquadCoefficients.cs` & `bosing-1.0.1/src/Bosing/BiquadCoefficients.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/BiquadFilter.cs` & `bosing-1.0.1/src/Bosing/BiquadFilter.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Bosing.csproj` & `bosing-1.0.1/src/Bosing/Bosing.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/BosingOptions.cs` & `bosing-1.0.1/src/Bosing/BosingOptions.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/ComplexReadOnlySpan.cs` & `bosing-1.0.1/src/Bosing/ComplexReadOnlySpan.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/ComplexSpan.cs` & `bosing-1.0.1/src/Bosing/ComplexSpan.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Envelope.cs` & `bosing-1.0.1/src/Bosing/Envelope.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/EnvelopeInfo.cs` & `bosing-1.0.1/src/Bosing/EnvelopeInfo.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/EnvelopeSample.cs` & `bosing-1.0.1/src/Bosing/EnvelopeSample.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/FirCoefficients.cs` & `bosing-1.0.1/src/Bosing/FirCoefficients.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/HannPulseShape.cs` & `bosing-1.0.1/src/Bosing/HannPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/IPulseShape.cs` & `bosing-1.0.1/src/Bosing/IPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/InterpolatedPulseShape.cs` & `bosing-1.0.1/src/Bosing/InterpolatedPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/IqPair.cs` & `bosing-1.0.1/src/Bosing/IqPair.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/MathUtils.cs` & `bosing-1.0.1/src/Bosing/MathUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/PhaseTrackingTransform.cs` & `bosing-1.0.1/src/Bosing/PhaseTrackingTransform.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/PooledComplexArray.cs` & `bosing-1.0.1/src/Bosing/PooledComplexArray.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/PostProcessTransform.cs` & `bosing-1.0.1/src/Bosing/PostProcessTransform.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/PulseList.cs` & `bosing-1.0.1/src/Bosing/PulseList.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/SignalFilter.cs` & `bosing-1.0.1/src/Bosing/SignalFilter.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/TimeAxisUtils.cs` & `bosing-1.0.1/src/Bosing/TimeAxisUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/ValueArray.cs` & `bosing-1.0.1/src/Bosing/ValueArray.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/WaveformSampler.cs` & `bosing-1.0.1/src/Bosing/WaveformSampler.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/WaveformUtils.cs` & `bosing-1.0.1/src/Bosing/WaveformUtils.cs`

 * *Files 1% similar despite different names*

```diff
@@ -20,26 +20,27 @@
                 foreach (var pulse in bin)
                 {
                     var delay = pulseList.TimeOffset + binKey.Delay;
                     var time = pulse.Time;
                     var tStart = time + delay;
                     var iFracStart = TimeAxisUtils.NextFracIndex(tStart, sampleRate, alignLevel);
                     var iStart = (int)Math.Ceiling(iFracStart);
-                    var envelopeInfo = new EnvelopeInfo(iStart - iFracStart, sampleRate);
+                    var indexOffset = iStart - iFracStart;
+                    var envelopeInfo = new EnvelopeInfo(indexOffset, sampleRate);
                     var envelopeSample = WaveformSampler<T>.GetEnvelopeSample(envelopeInfo, binKey.Envelope);
                     if (envelopeSample is null)
                     {
                         continue;
                     }
 
                     var globalFrequency = binKey.GlobalFrequency - loFrequency;
                     var localFrequency = binKey.LocalFrequency;
                     var totalFrequency = globalFrequency + localFrequency;
                     var dt = 1 / sampleRate;
-                    var phaseShift = Math.Tau * globalFrequency * (iStart * dt - delay);
+                    var phaseShift = Math.Tau * (globalFrequency * (iStart * dt - delay) + localFrequency * indexOffset * dt);
                     var amplitude = pulse.Amplitude * pulseList.AmplitudeMultiplier * Complex.FromPolarCoordinates(1, phaseShift);
                     var complexAmplitude = amplitude.Amplitude;
                     var dragAmplitude = amplitude.DragAmplitude * sampleRate;
                     var dPhase = T.CreateChecked(Math.Tau * totalFrequency * dt);
                     MixAddEnvelope(tempWaveform[iStart..], envelopeSample, (IqPair<T>)complexAmplitude, (IqPair<T>)dragAmplitude, dPhase);
                 }
             }
```

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/AbsoluteSchedule.cs` & `bosing-1.0.1/src/Bosing/Schedules/AbsoluteSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/BarrierElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/BarrierElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/GridLength.cs` & `bosing-1.0.1/src/Bosing/Schedules/GridLength.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/GridSchedule.cs` & `bosing-1.0.1/src/Bosing/Schedules/GridSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/PlayElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/PlayElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/RepeatElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/RepeatElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/Schedule.cs` & `bosing-1.0.1/src/Bosing/Schedules/Schedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/ScheduleElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/ScheduleElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/SetFrequencyElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/SetFrequencyElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/SetPhaseElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/SetPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/ShiftFrequencyElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/ShiftFrequencyElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/ShiftPhaseElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/ShiftPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/StackSchedule.cs` & `bosing-1.0.1/src/Bosing/Schedules/StackSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing/Schedules/SwapPhaseElement.cs` & `bosing-1.0.1/src/Bosing/Schedules/SwapPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Api.cs` & `bosing-1.0.1/src/Bosing.Aot/Api.cs`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 using System.Runtime.InteropServices;
 
-using MessagePack;
-
 using Bosing.Aot.Models;
 
+using MessagePack;
+
 namespace Bosing.Aot;
 
 public static class Api
 {
     private static MessagePackSerializerOptions MessagePackSerializerOptions { get; } =
         new MessagePackSerializerOptions(GeneratedMessagePackResolver.InstanceWithStandardAotResolver);
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Bosing.Aot.csproj` & `bosing-1.0.1/src/Bosing.Aot/Bosing.Aot.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/ScheduleRunner.cs` & `bosing-1.0.1/src/Bosing.Aot/ScheduleRunner.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 using System.Diagnostics;
 
-using CommunityToolkit.Diagnostics;
-
 using Bosing.Aot.Models;
 
+using CommunityToolkit.Diagnostics;
+
 namespace Bosing.Aot;
 
 public sealed class ScheduleRunner
 {
     private readonly ScheduleRequest _scheduleRequest;
     private readonly BosingOptions _options = new();
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+using Bosing.Schedules;
+
 using CommunityToolkit.Diagnostics;
 
 using MessagePack;
 
-using Bosing.Schedules;
-
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class AbsoluteScheduleDto : ScheduleElementDto
 {
     [Key(6)]
     public IList<(double Time, ScheduleElementDto Element)>? Elements { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/BarrierElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-using CommunityToolkit.Diagnostics;
+using Bosing.Schedules;
 
 using MessagePack;
 
-using Bosing.Schedules;
-
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
-public sealed class BarrierElementDto : ScheduleElementDto
+public sealed class ShiftPhaseElementDto : ScheduleElementDto
 {
     [Key(6)]
-    public ISet<int>? ChannelIds { get; set; }
+    public int ChannelId { get; set; }
+    [Key(7)]
+    public double DeltaPhase { get; set; }
 
     public override ScheduleElement GetScheduleElement(ScheduleRequest request)
     {
-        Guard.IsNotNull(ChannelIds);
-        return new BarrierElement(ChannelIds)
+        return new ShiftPhaseElement(ChannelId, DeltaPhase)
         {
             Margin = Margin,
             Alignment = Alignment,
             IsVisible = IsVisible,
             Duration = Duration,
             MaxDuration = MaxDuration,
             MinDuration = MinDuration,
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/BiquadDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/BiquadDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/GridScheduleDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/GridScheduleDto.cs`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+using Bosing.Schedules;
+
 using CommunityToolkit.Diagnostics;
 
 using MessagePack;
 
-using Bosing.Schedules;
-
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class GridScheduleDto : ScheduleElementDto
 {
     [Key(6)]
     public IList<(int Column, int Span, ScheduleElementDto Element)>? Elements { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/OptionsDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/OptionsDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/PlayElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/PlayElementDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 using System.Diagnostics;
 
-using MessagePack;
-
 using Bosing.Schedules;
 
+using MessagePack;
+
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class PlayElementDto : ScheduleElementDto
 {
     [Key(6)]
     public int ChannelId { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/RepeatElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/RepeatElementDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+using Bosing.Schedules;
+
 using CommunityToolkit.Diagnostics;
 
 using MessagePack;
 
-using Bosing.Schedules;
-
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class RepeatElementDto : ScheduleElementDto
 {
     [Key(6)]
     public ScheduleElementDto? Element { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/ScheduleElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/ScheduleElementDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-using MessagePack;
-
 using Bosing.Schedules;
 
+using MessagePack;
+
 namespace Bosing.Aot.Models;
 
 
 [Union(0, typeof(PlayElementDto))]
 [Union(1, typeof(ShiftPhaseElementDto))]
 [Union(2, typeof(SetPhaseElementDto))]
 [Union(3, typeof(ShiftFrequencyElementDto))]
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/SetFrequencyElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/SetFrequencyElementDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-using MessagePack;
-
 using Bosing.Schedules;
 
+using MessagePack;
+
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class SetFrequencyElementDto : ScheduleElementDto
 {
     [Key(6)]
     public int ChannelId { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/SetPhaseElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/SetPhaseElementDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-using MessagePack;
-
 using Bosing.Schedules;
 
+using MessagePack;
+
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class SetPhaseElementDto : ScheduleElementDto
 {
     [Key(6)]
     public int ChannelId { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-using MessagePack;
-
 using Bosing.Schedules;
 
+using MessagePack;
+
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class ShiftFrequencyElementDto : ScheduleElementDto
 {
     [Key(6)]
     public int ChannelId { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/StackScheduleDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/StackScheduleDto.cs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+using Bosing.Schedules;
+
 using CommunityToolkit.Diagnostics;
 
 using MessagePack;
 
-using Bosing.Schedules;
-
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class StackScheduleDto : ScheduleElementDto
 {
     [Key(6)]
     public IList<ScheduleElementDto>? Elements { get; set; }
```

### Comparing `bosing-1.0.0b4/src/Bosing.Aot/Models/SwapPhaseElementDto.cs` & `bosing-1.0.1/src/Bosing.Aot/Models/SwapPhaseElementDto.cs`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-using MessagePack;
-
 using Bosing.Schedules;
 
+using MessagePack;
+
 namespace Bosing.Aot.Models;
 
 [MessagePackObject]
 public sealed class SwapPhaseElementDto : ScheduleElementDto
 {
     [Key(6)]
     public int ChannelId1 { get; set; }
```

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Bosing.Tests.csproj` & `bosing-1.0.1/tests/Bosing.Tests/Bosing.Tests.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/EnvelopeInfoTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/EnvelopeInfoTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/HannPulseShapeTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/HannPulseShapeTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/IntegrationTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/IntegrationTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/IqPairTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/IqPairTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/PooledComplexArrayTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/PooledComplexArrayTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/PulseListTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/PulseListTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/TimeAxisUtilsTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/TimeAxisUtilsTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/TrianglePulseShapeTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/TrianglePulseShapeTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/WaveformUtilsTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/WaveformUtilsTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/GridScheduleTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/GridScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/RepeatElementTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/RepeatElementTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/ScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/StackScheduleTests.cs` & `bosing-1.0.1/tests/Bosing.Tests/Schedules/StackScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/.gitignore` & `bosing-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/LICENSE.txt` & `bosing-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b4/README.md` & `bosing-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,31 +40,32 @@
 ### Run tests
 
 ```bash
 dotnet test
 hatch run test:run
 ```
 
-### Usage (TODO)
+### Usage
 
 Examples can be found in `python/examples`.
 
 ```python
-from bosing import Play, Hann, Channel, Stack, generate_waveforms
+from bosing import Play, Barrier, Hann, Channel, Stack, generate_waveforms
 import matplotlib.pyplot as plt
 
 channels = [Channel("xy", 200e6, 2e9, 100000)]
 shapes = [Hann()]
-schedule = Stack(duration=49.9e-6).with_children(
+schedule = Stack(duration=50e-6).with_children(
     Play(
         channel_id = 0,
         amplitude = 0.3,
         shape_id = 0,
         width = 100e-9,
-    )
+    ),
+    Barrier(duration=10e-9),
 )
 result = generate_waveforms(channels, shapes, schedule)
 i, q = result["xy"]
 plt.plot(i)
 plt.plot(q)
 plt.show()
 ```
```

### Comparing `bosing-1.0.0b4/hatch_build.py` & `bosing-1.0.1/hatch_build.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,20 +71,14 @@
     if plat_tag is None:
         plat_tag = sysconfig.get_platform().replace("-", "_").replace(".", "_")
     return f"py3-none-{plat_tag}"
 
 
 class CustomBuildHook(BuildHookInterface):
     def initialize(self, version: str, build_data: Dict[str, Any]) -> None:
-        # Skip building the C# library when building the docs
-        if (
-            os.environ.get("HATCH_ENV_ACTIVE") == "docs"
-            or os.environ.get("READTHEDOCS") == "True"
-        ):
-            return
         if self.target_name == "wheel":
             _dotnet_publish(version, build_data)
             build_data["pure_python"] = False
             build_data["tag"] = _infer_tag()
 
     def clean(self, versions: List[str]) -> None:
         shutil.rmtree(DST_DIR, ignore_errors=True)
```

### Comparing `bosing-1.0.0b4/pyproject.toml` & `bosing-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 [tool.hatch.build.targets.wheel]
 packages = ["python/bosing"]
 
 [tool.hatch.envs.default]
 dependencies = ["scipy", "matplotlib", "ipython"]
 
 [tool.hatch.envs.docs]
-dependencies = ["sphinx", "furo"]
+dependencies = ["sphinx", "furo", "matplotlib"]
 
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -M html python/docs python/docs/_build {args}"
 clean = "rm -rf python/docs/_build docs/_autosummary"
 
 [tool.hatch.envs.docs.overrides]
 platform.windows.scripts = [
@@ -62,7 +62,14 @@
 run = "pytest {args}"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 testpaths = ["python/tests"]
+
+[tool.hatch.envs.hatch-static-analysis]
+config-path = "ruff_defaults.toml"
+
+[tool.ruff]
+extend = "ruff_defaults.toml"
+include = ["python/bosing/*.py", "python/tests/*.py"]
```

### Comparing `bosing-1.0.0b4/PKG-INFO` & `bosing-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 1.0.0b4
+Version: 1.0.1
 Summary: Waveform generator for pulse sequences in quantum computing
 Project-URL: Documentation, https://github.com/kahojyun/Bosing#readme
 Project-URL: Issues, https://github.com/kahojyun/Bosing/issues
 Project-URL: Source, https://github.com/kahojyun/Bosing
 Author-email: kaho <kaho0769@qq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -64,31 +64,32 @@
 ### Run tests
 
 ```bash
 dotnet test
 hatch run test:run
 ```
 
-### Usage (TODO)
+### Usage
 
 Examples can be found in `python/examples`.
 
 ```python
-from bosing import Play, Hann, Channel, Stack, generate_waveforms
+from bosing import Play, Barrier, Hann, Channel, Stack, generate_waveforms
 import matplotlib.pyplot as plt
 
 channels = [Channel("xy", 200e6, 2e9, 100000)]
 shapes = [Hann()]
-schedule = Stack(duration=49.9e-6).with_children(
+schedule = Stack(duration=50e-6).with_children(
     Play(
         channel_id = 0,
         amplitude = 0.3,
         shape_id = 0,
         width = 100e-9,
-    )
+    ),
+    Barrier(duration=10e-9),
 )
 result = generate_waveforms(channels, shapes, schedule)
 i, q = result["xy"]
 plt.plot(i)
 plt.plot(q)
 plt.show()
 ```
```

