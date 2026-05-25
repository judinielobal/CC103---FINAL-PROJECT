package bombrush;

import javax.sound.sampled.*;

public class AudioPlayer {

    public static void play(String path) {

        try {
            AudioInputStream audio =
                    AudioSystem.getAudioInputStream(AudioPlayer.class.getResource(path));

            Clip clip = AudioSystem.getClip();
            clip.open(audio);
            clip.start();

        } catch (Exception e) {
            System.out.println("Audio error: " + e.getMessage());
        }
    }
}
