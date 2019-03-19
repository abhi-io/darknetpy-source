


    pip install darknetpy


Usage
====================

In example.py::

    from darknetpy.detector import Detector

    detector = Detector('<absolute-path-to>/darknet/cfg/coco.data',
                        '<absolute-path-to>/darknet/cfg/yolo.cfg',
                        '<absolute-path-to>/darknet/yolo.weights')

    results = detector.detect('<absolute-path-to>/darknet/data/dog.jpg')

    print(results)

Runing::

    python example.py


Result::

    [{'right': 194, 'bottom': 353, 'top': 264, 'class': 'dog', 'prob': 0.8198755383491516, 'left': 71}]
