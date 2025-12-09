---
layout: default
title: Virtual Exhibition
permalink: /exhibition/
---

<section class="exhibition-page">
  <div class="container">
    <!-- Museum Entrance -->
    <header class="museum-entrance">
      <div class="entrance-content">
        <h1 class="museum-title">Virtual Photography Museum</h1>
        <p class="museum-subtitle">Step into a digital gallery experience. Navigate through rooms to explore different photography series.</p>
        
        <div class="entrance-actions">
          <button class="btn btn-primary" id="enter-museum">
            Enter Exhibition
          </button>
          <div class="visitor-count">
            <span class="count-icon">👥</span>
            <span id="visitor-count">Loading...</span> visitors currently viewing
          </div>
        </div>
        
        <div class="exhibition-guide">
          <h3>How to Navigate</h3>
          <div class="guide-steps">
            <div class="step">
              <div class="step-number">1</div>
              <p>Use <strong>arrow keys</strong> or <strong>WASD</strong> to move through the gallery</p>
            </div>
            <div class="step">
              <div class="step-number">2</div>
              <p><strong>Click on photos</strong> to view them in detail</p>
            </div>
            <div class="step">
              <div class="step-number">3</div>
              <p>Press <strong>ESC</strong> to exit fullscreen view</p>
            </div>
          </div>
        </div>
      </div>
    </header>

    <!-- Museum Gallery (Initially Hidden) -->
    <div class="museum-gallery" id="museum-gallery" style="display: none;">
      <!-- Museum Controls -->
      <div class="museum-controls">
        <button class="control-btn" id="toggle-fullscreen" title="Toggle Fullscreen">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none">
            <path d="M8 3H5C3.89543 3 3 3.89543 3 5V8M21 8V5C21 3.89543 20.1046 3 19 3H16M16 21H19C20.1046 21 21 20.1046 21 19V16M3 16V19C3 20.1046 3.89543 21 5 21H8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </button>
        
        <div class="room-info">
          <h3 id="current-room">Gallery Entrance</h3>
          <div class="room-counter">
            Room <span id="room-number">1</span> of <span id="total-rooms">4</span>
          </div>
        </div>
        
        <button class="control-btn" id="exit-museum" title="Exit Museum">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none">
            <path d="M18 6L6 18M6 6L18 18" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </button>
      </div>

      <!-- Gallery Rooms -->
      <div class="gallery-rooms">
        <!-- Room 1: Street Photography -->
        <div class="museum-room active" id="room-1" data-room="street">
          <div class="room-header">
            <h2>Street Photography</h2>
            <p class="room-description">Urban moments and candid street scenes</p>
          </div>
          
          <div class="room-layout">
            <!-- Left Wall -->
            <div class="gallery-wall left-wall">
              <div class="artwork" data-index="0" style="top: 20%; left: 15%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/400/600?random=1" alt="Street Scene 1" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Morning Commute</span>
                    <span class="artwork-info">Downtown, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Center Wall -->
            <div class="gallery-wall center-wall">
              <div class="artwork featured" data-index="1" style="top: 15%; left: 35%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/500/700?random=2" alt="Street Scene 2" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Urban Rhythm</span>
                    <span class="artwork-info">City Center, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Right Wall -->
            <div class="gallery-wall right-wall">
              <div class="artwork" data-index="2" style="top: 25%; left: 60%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/400/550?random=3" alt="Street Scene 3" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Evening Shadows</span>
                    <span class="artwork-info">Financial District, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Navigation Arrows -->
            <div class="room-nav next-room" data-target="room-2">
              <span class="nav-arrow">→</span>
              <span class="nav-label">Portrait Gallery</span>
            </div>
          </div>
        </div>

        <!-- Room 2: Portrait Gallery -->
        <div class="museum-room" id="room-2" data-room="portrait">
          <div class="room-header">
            <h2>Portrait Gallery</h2>
            <p class="room-description">Intimate portraits and character studies</p>
          </div>
          
          <div class="room-layout">
            <!-- Left Wall -->
            <div class="gallery-wall left-wall">
              <div class="artwork" data-index="3" style="top: 30%; left: 20%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/450/600?random=4" alt="Portrait 1" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Contemplation</span>
                    <span class="artwork-info">Studio Portrait, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Center Wall -->
            <div class="gallery-wall center-wall">
              <div class="artwork featured" data-index="4" style="top: 20%; left: 40%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/500/650?random=5" alt="Portrait 2" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">The Artist</span>
                    <span class="artwork-info">Natural Light, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Navigation Arrows -->
            <div class="room-nav prev-room" data-target="room-1">
              <span class="nav-arrow">←</span>
              <span class="nav-label">Street Gallery</span>
            </div>
            
            <div class="room-nav next-room" data-target="room-3">
              <span class="nav-arrow">→</span>
              <span class="nav-label">Landscape Wing</span>
            </div>
          </div>
        </div>

        <!-- Room 3: Landscape Wing -->
        <div class="museum-room" id="room-3" data-room="landscape">
          <div class="room-header">
            <h2>Landscape Wing</h2>
            <p class="room-description">Natural landscapes and scenic vistas</p>
          </div>
          
          <div class="room-layout">
            <!-- Center Wall (Panoramic) -->
            <div class="gallery-wall center-wall panoramic">
              <div class="artwork panoramic" data-index="5" style="top: 25%; left: 30%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/800/400?random=6" alt="Landscape 1" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Mountain Dawn</span>
                    <span class="artwork-info">Alpine Region, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Navigation Arrows -->
            <div class="room-nav prev-room" data-target="room-2">
              <span class="nav-arrow">←</span>
              <span class="nav-label">Portrait Gallery</span>
            </div>
            
            <div class="room-nav next-room" data-target="room-4">
              <span class="nav-arrow">→</span>
              <span class="nav-label">Special Exhibition</span>
            </div>
          </div>
        </div>

        <!-- Room 4: Special Exhibition -->
        <div class="museum-room" id="room-4" data-room="special">
          <div class="room-header">
            <h2>Special Exhibition</h2>
            <p class="room-description">Experimental and conceptual work</p>
          </div>
          
          <div class="room-layout">
            <!-- Multi-wall installation -->
            <div class="installation">
              <div class="artwork" data-index="6" style="top: 15%; left: 20%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/400/500?random=7" alt="Conceptual 1" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Abstraction #1</span>
                    <span class="artwork-info">Mixed Media, 2023</span>
                  </div>
                </div>
              </div>
              
              <div class="artwork" data-index="7" style="top: 15%; left: 50%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/400/500?random=8" alt="Conceptual 2" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Abstraction #2</span>
                    <span class="artwork-info">Digital Composite, 2023</span>
                  </div>
                </div>
              </div>
              
              <div class="artwork" data-index="8" style="top: 60%; left: 35%;">
                <div class="artwork-frame">
                  <img src="https://picsum.photos/500/300?random=9" alt="Conceptual 3" class="artwork-image">
                  <div class="artwork-label">
                    <span class="artwork-title">Urban Geometry</span>
                    <span class="artwork-info">Architectural Study, 2023</span>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Navigation Arrow -->
            <div class="room-nav prev-room" data-target="room-3">
              <span class="nav-arrow">←</span>
              <span class="nav-label">Landscape Wing</span>
            </div>
            
            <div class="room-exit">
              <button class="btn btn-outline" id="exit-to-lobby">
                Exit to Lobby
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- Visitor Position -->
      <div class="visitor-position">
        <div class="position-dot"></div>
      </div>

      <!-- Detailed View Modal -->
      <div class="detail-modal" id="detail-modal">
        <div class="modal-content">
          <button class="modal-close" id="modal-close">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none">
              <path d="M18 6L6 18M6 6L18 18" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            </svg>
          </button>
          
          <div class="modal-image-container">
            <img id="modal-image" src="" alt="" class="modal-image">
          </div>
          
          <div class="modal-details">
            <h3 id="modal-title">Artwork Title</h3>
            <p id="modal-description">Artwork description goes here</p>
            
            <div class="modal-meta">
              <div class="meta-item">
                <strong>Series:</strong>
                <span id="modal-series">Street Photography</span>
              </div>
              <div class="meta-item">
                <strong>Location:</strong>
                <span id="modal-location">City Center</span>
              </div>
              <div class="meta-item">
                <strong>Date:</strong>
                <span id="modal-date">2023</span>
              </div>
              <div class="meta-item">
                <strong>Equipment:</strong>
                <span id="modal-equipment">Fujifilm X-T4, 35mm</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
.exhibition-page {
  padding: 80px 0 0;
  min-height: 100vh;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
}

.container {
  max-width: 1400px;
}

/* Museum Entrance */
.museum-entrance {
  text-align: center;
  padding: 4rem 2rem;
  max-width: 800px;
  margin: 0 auto;
}

.museum-title {
  font-size: 3.5rem;
  font-weight: 300;
  margin-bottom: 1.5rem;
  letter-spacing: 0.5px;
  text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
}

.museum-subtitle {
  font-size: 1.25rem;
  opacity: 0.9;
  margin-bottom: 3rem;
  line-height: 1.6;
}

.entrance-actions {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
  margin-bottom: 4rem;
}

#enter-museum {
  padding: 1rem 3rem;
  font-size: 1.25rem;
  background: white;
  color: #667eea;
  border: none;
  border-radius: 50px;
  cursor: pointer;
  transition: all 0.3s ease;
}

#enter-museum:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
}

.visitor-count {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  font-size: 1rem;
  opacity: 0.8;
}

.count-icon {
  font-size: 1.25rem;
}

/* Exhibition Guide */
.exhibition-guide {
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border-radius: 20px;
  padding: 2.5rem;
  margin-top: 2rem;
  border: 1px solid rgba(255, 255, 255, 0.2);
}

.exhibition-guide h3 {
  font-size: 1.5rem;
  margin-bottom: 2rem;
  font-weight: 400;
}

.guide-steps {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.step {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 1rem;
}

.step-number {
  width: 40px;
  height: 40px;
  background: white;
  color: #667eea;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 1.25rem;
}

.step p {
  opacity: 0.9;
  line-height: 1.5;
}

/* Museum Gallery */
.museum-gallery {
  background: linear-gradient(to bottom, #1a1a2e, #16213e);
  min-height: 100vh;
  position: relative;
  overflow: hidden;
}

.museum-controls {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background: rgba(0, 0, 0, 0.8);
  backdrop-filter: blur(10px);
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 1000;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.control-btn {
  background: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.2);
  color: white;
  width: 40px;
  height: 40px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.3s ease;
}

.control-btn:hover {
  background: rgba(255, 255, 255, 0.2);
  transform: scale(1.05);
}

.room-info {
  text-align: center;
}

.room-info h3 {
  font-size: 1.25rem;
  font-weight: 400;
  margin-bottom: 0.25rem;
}

.room-counter {
  font-size: 0.875rem;
  opacity: 0.7;
}

/* Gallery Rooms */
.gallery-rooms {
  position: relative;
  min-height: calc(100vh - 80px);
  margin-top: 80px;
}

.museum-room {
  display: none;
  padding: 2rem;
  position: relative;
  height: calc(100vh - 120px);
}

.museum-room.active {
  display: block;
  animation: fadeIn 0.5s ease;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.room-header {
  text-align: center;
  margin-bottom: 2rem;
  padding: 0 2rem;
}

.room-header h2 {
  font-size: 2.5rem;
  font-weight: 300;
  margin-bottom: 0.5rem;
  letter-spacing: 0.5px;
}

.room-description {
  font-size: 1.125rem;
  opacity: 0.8;
}

/* Room Layout */
.room-layout {
  position: relative;
  height: 70vh;
  background: linear-gradient(to bottom, rgba(255,255,255,0.05), transparent);
  border-radius: 20px;
  overflow: hidden;
}

.gallery-wall {
  position: absolute;
  height: 100%;
  background: linear-gradient(to bottom, #2d3047, #1f2235);
  border: 1px solid rgba(255, 255, 255, 0.1);
}

.left-wall {
  width: 30%;
  left: 5%;
  transform: perspective(1000px) rotateY(10deg);
}

.center-wall {
  width: 40%;
  left: 30%;
  z-index: 2;
  box-shadow: 0 0 50px rgba(0, 0, 0, 0.5);
}

.center-wall.panoramic {
  width: 60%;
  left: 20%;
}

.right-wall {
  width: 30%;
  right: 5%;
  transform: perspective(1000px) rotateY(-10deg);
}

/* Artworks */
.artwork {
  position: absolute;
  cursor: pointer;
  transition: all 0.3s ease;
}

.artwork:hover {
  transform: translateY(-5px) scale(1.02);
  z-index: 10;
}

.artwork.featured {
  z-index: 5;
}

.artwork-frame {
  background: white;
  padding: 10px;
  border-radius: 8px;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
}

.artwork-image {
  width: 100%;
  height: auto;
  display: block;
  border-radius: 4px;
}

.artwork-label {
  background: rgba(0, 0, 0, 0.8);
  color: white;
  padding: 0.75rem;
  border-radius: 4px;
  margin-top: 0.5rem;
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
}

.artwork-title {
  font-weight: 600;
  font-size: 0.875rem;
}

.artwork-info {
  font-size: 0.75rem;
  opacity: 0.8;
}

/* Navigation Arrows */
.room-nav {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  color: white;
  padding: 1rem 1.5rem;
  border-radius: 50px;
  display: flex;
  align-items: center;
  gap: 0.75rem;
  cursor: pointer;
  transition: all 0.3s ease;
  z-index: 100;
}

.room-nav:hover {
  background: rgba(255, 255, 255, 0.2);
  transform: translateY(-50%) scale(1.05);
}

.prev-room {
  left: 2rem;
}

.next-room {
  right: 2rem;
}

.nav-arrow {
  font-size: 1.5rem;
}

.nav-label {
  font-size: 0.875rem;
}

.room-exit {
  position: absolute;
  bottom: 2rem;
  left: 50%;
  transform: translateX(-50%);
}

/* Visitor Position */
.visitor-position {
  position: fixed;
  bottom: 2rem;
  left: 50%;
  transform: translateX(-50%);
  z-index: 1000;
}

.position-dot {
  width: 20px;
  height: 20px;
  background: rgba(255, 255, 255, 0.8);
  border-radius: 50%;
  box-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.2); }
}

/* Installation Layout */
.installation {
  position: relative;
  height: 100%;
}

/* Detail Modal */
.detail-modal {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.95);
  z-index: 2000;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.detail-modal.active {
  display: flex;
  animation: fadeIn 0.3s ease;
}

.modal-content {
  background: #1a1a2e;
  border-radius: 20px;
  max-width: 1200px;
  max-height: 90vh;
  overflow: hidden;
  position: relative;
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 0;
}

.modal-close {
  position: absolute;
  top: 1rem;
  right: 1rem;
  background: rgba(255, 255, 255, 0.1);
  border: none;
  color: white;
  width: 40px;
  height: 40px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  z-index: 10;
  transition: all 0.3s ease;
}

.modal-close:hover {
  background: rgba(255, 255, 255, 0.2);
}

.modal-image-container {
  padding: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #000;
}

.modal-image {
  max-width: 100%;
  max-height: 70vh;
  object-fit: contain;
}

.modal-details {
  padding: 2rem;
  overflow-y: auto;
}

.modal-details h3 {
  font-size: 1.75rem;
  margin-bottom: 1rem;
  font-weight: 400;
}

.modal-details p {
  margin-bottom: 2rem;
  line-height: 1.6;
  opacity: 0.9;
}

.modal-meta {
  display: grid;
  gap: 1rem;
}

.meta-item {
  padding-bottom: 1rem;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.meta-item strong {
  display: block;
  margin-bottom: 0.25rem;
  font-size: 0.875rem;
  opacity: 0.7;
}

/* Responsive Design */
@media (max-width: 1024px) {
  .museum-title {
    font-size: 2.5rem;
  }
  
  .modal-content {
    grid-template-columns: 1fr;
    max-height: 95vh;
  }
  
  .modal-image {
    max-height: 50vh;
  }
}

@media (max-width: 768px) {
  .exhibition-page {
    padding: 60px 0 0;
  }
  
  .museum-title {
    font-size: 2rem;
  }
  
  .museum-subtitle {
    font-size: 1.125rem;
  }
  
  .guide-steps {
    grid-template-columns: 1fr;
  }
  
  .room-header h2 {
    font-size: 2rem;
  }
  
  .room-layout {
    height: 60vh;
  }
  
  .left-wall, .right-wall {
    display: none;
  }
  
  .center-wall {
    width: 80%;
    left: 10%;
    transform: none;
  }
  
  .room-nav {
    padding: 0.75rem 1rem;
  }
  
  .nav-label {
    display: none;
  }
}

@media (max-width: 480px) {
  .museum-entrance {
    padding: 2rem 1rem;
  }
  
  .exhibition-guide {
    padding: 1.5rem;
  }
  
  .museum-controls {
    padding: 1rem;
  }
  
  .modal-details {
    padding: 1.5rem;
  }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Museum State
  let currentRoom = 'room-1';
  let visitorCount = Math.floor(Math.random() * 50) + 10;
  let isFullscreen = false;
  
  // DOM Elements
  const entrance = document.querySelector('.museum-entrance');
  const gallery = document.getElementById('museum-gallery');
  const enterBtn = document.getElementById('enter-museum');
  const exitBtn = document.getElementById('exit-museum');
  const fullscreenBtn = document.getElementById('toggle-fullscreen');
  const rooms = document.querySelectorAll('.museum-room');
  const artworks = document.querySelectorAll('.artwork');
  const detailModal = document.getElementById('detail-modal');
  const modalClose = document.getElementById('modal-close');
  const exitToLobby = document.getElementById('exit-to-lobby');
  const visitorCountEl = document.getElementById('visitor-count');
  
  // Initialize
  updateVisitorCount();
  setupEventListeners();
  
  function updateVisitorCount() {
    visitorCountEl.textContent = visitorCount;
  }
  
  function setupEventListeners() {
    // Enter Museum
    enterBtn.addEventListener('click', enterMuseum);
    
    // Exit Museum
    exitBtn.addEventListener('click', exitMuseum);
    exitToLobby.addEventListener('click', exitMuseum);
    
    // Fullscreen Toggle
    fullscreenBtn.addEventListener('click', toggleFullscreen);
    
    // Room Navigation
    document.querySelectorAll('.room-nav').forEach(nav => {
      nav.addEventListener('click', function() {
        const targetRoom = this.getAttribute('data-target');
        navigateToRoom(targetRoom);
      });
    });
    
    // Artwork Click
    artworks.forEach(artwork => {
      artwork.addEventListener('click', function() {
        const index = this.getAttribute('data-index');
        showArtworkDetail(index);
      });
    });
    
    // Modal Close
    modalClose.addEventListener('click', closeModal);
    detailModal.addEventListener('click', function(e) {
      if (e.target === this) closeModal();
    });
    
    // Keyboard Navigation
    document.addEventListener('keydown', handleKeyNavigation);
    
    // Prevent scroll in museum
    gallery.addEventListener('wheel', preventScroll, { passive: false });
  }
  
  function enterMuseum() {
    entrance.style.display = 'none';
    gallery.style.display = 'block';
    document.body.style.overflow = 'hidden';
    
    // Simulate visitor joining
    visitorCount++;
    updateVisitorCount();
    
    // Start room
    navigateToRoom('room-1');
  }
  
  function exitMuseum() {
    gallery.style.display = 'none';
    entrance.style.display = 'block';
    document.body.style.overflow = 'auto';
    
    // Exit fullscreen if active
    if (isFullscreen) {
      exitFullscreen();
    }
    
    // Reset room
    navigateToRoom('room-1');
  }
  
  function navigateToRoom(roomId) {
    // Hide current room
    rooms.forEach(room => {
      room.classList.remove('active');
    });
    
    // Show new room
    const newRoom = document.getElementById(roomId);
    if (newRoom) {
      newRoom.classList.add('active');
      currentRoom = roomId;
      
      // Update room info
      updateRoomInfo();
      
      // Add entrance animation
      newRoom.style.animation = 'fadeIn 0.5s ease';
    }
  }
  
  function updateRoomInfo() {
    const roomNumber = parseInt(currentRoom.split('-')[1]);
    const roomName = document.querySelector(`#${currentRoom} h2`).textContent;
    
    document.getElementById('current-room').textContent = roomName;
    document.getElementById('room-number').textContent = roomNumber;
    document.getElementById('total-rooms').textContent = rooms.length;
  }
  
  function showArtworkDetail(index) {
    // In a real implementation, you would fetch artwork data
    const artworkData = {
      0: {
        title: 'Morning Commute',
        description: 'A candid street photograph capturing the energy of morning rush hour in the city center.',
        series: 'Street Photography',
        location: 'Downtown Financial District',
        date: 'Spring 2023',
        equipment: 'Fujifilm X-T4, 35mm f/2',
        image: 'https://picsum.photos/800/1200?random=1'
      },
      1: {
        title: 'Urban Rhythm',
        description: 'Study of movement and light in the city, showcasing the dynamic nature of urban life.',
        series: 'Street Photography',
        location: 'City Center',
        date: 'Summer 2023',
        equipment: 'Sony A7III, 24-70mm f/2.8',
        image: 'https://picsum.photos/800/1200?random=2'
      },
      2: {
        title: 'Evening Shadows',
        description: 'Play of light and shadow during golden hour in the financial district.',
        series: 'Street Photography',
        location: 'Financial District',
        date: 'Fall 2023',
        equipment: 'Canon R5, 85mm f/1.8',
        image: 'https://picsum.photos/800/1200?random=3'
      },
      3: {
        title: 'Contemplation',
        description: 'Portrait session in natural light, capturing a moment of quiet reflection.',
        series: 'Portrait Gallery',
        location: 'Studio',
        date: 'Winter 2023',
        equipment: 'Fujifilm X-T4, 56mm f/1.2',
        image: 'https://picsum.photos/800/1200?random=4'
      },
      4: {
        title: 'The Artist',
        description: 'Environmental portrait of a local artist in their creative workspace.',
        series: 'Portrait Gallery',
        location: 'Artist Studio',
        date: 'Spring 2023',
        equipment: 'Sony A7III, 35mm f/1.4',
        image: 'https://picsum.photos/800/1200?random=5'
      },
      5: {
        title: 'Mountain Dawn',
        description: 'Panoramic landscape capturing the first light of day on mountain peaks.',
        series: 'Landscape Wing',
        location: 'Alpine Region',
        date: 'Summer 2023',
        equipment: 'Canon R5, 16-35mm f/2.8',
        image: 'https://picsum.photos/1200/600?random=6'
      },
      6: {
        title: 'Abstraction #1',
        description: 'Experimental photography exploring form, color, and texture.',
        series: 'Special Exhibition',
        location: 'Digital Studio',
        date: '2023',
        equipment: 'Mixed Media, Digital Composite',
        image: 'https://picsum.photos/800/1200?random=7'
      },
      7: {
        title: 'Abstraction #2',
        description: 'Digital composite exploring the boundaries between photography and digital art.',
        series: 'Special Exhibition',
        location: 'Digital Studio',
        date: '2023',
        equipment: 'Digital Composite, Photoshop',
        image: 'https://picsum.photos/800/1200?random=8'
      },
      8: {
        title: 'Urban Geometry',
        description: 'Architectural study focusing on geometric patterns in urban environments.',
        series: 'Special Exhibition',
        location: 'City Center',
        date: '2023',
        equipment: 'Fujifilm X-T4, 23mm f/2',
        image: 'https://picsum.photos/1200/800?random=9'
      }
    };
    
    const data = artworkData[index] || artworkData[0];
    
    // Update modal content
    document.getElementById('modal-title').textContent = data.title;
    document.getElementById('modal-description').textContent = data.description;
    document.getElementById('modal-series').textContent = data.series;
    document.getElementById('modal-location').textContent = data.location;
    document.getElementById('modal-date').textContent = data.date;
    document.getElementById('modal-equipment').textContent = data.equipment;
    document.getElementById('modal-image').src = data.image;
    document.getElementById('modal-image').alt = data.title;
    
    // Show modal
    detailModal.classList.add('active');
    document.body.style.overflow = 'hidden';
  }
  
  function closeModal() {
    detailModal.classList.remove('active');
    document.body.style.overflow = 'hidden';
  }
  
  function handleKeyNavigation(e) {
    if (!gallery.style.display || gallery.style.display === 'none') return;
    
    switch(e.key.toLowerCase()) {
      case 'arrowleft':
      case 'a':
        navigateToPreviousRoom();
        break;
      case 'arrowright':
      case 'd':
        navigateToNextRoom();
        break;
      case 'escape':
        closeModal();
        if (isFullscreen) exitFullscreen();
        break;
      case 'f':
        toggleFullscreen();
        break;
    }
  }
  
  function navigateToPreviousRoom() {
    const currentNum = parseInt(currentRoom.split('-')[1]);
    if (currentNum > 1) {
      navigateToRoom(`room-${currentNum - 1}`);
    }
  }
  
  function navigateToNextRoom() {
    const currentNum = parseInt(currentRoom.split('-')[1]);
    if (currentNum < rooms.length) {
      navigateToRoom(`room-${currentNum + 1}`);
    }
  }
  
  function toggleFullscreen() {
    if (!isFullscreen) {
      enterFullscreen();
    } else {
      exitFullscreen();
    }
  }
  
  function enterFullscreen() {
    const elem = gallery;
    if (elem.requestFullscreen) {
      elem.requestFullscreen();
    } else if (elem.webkitRequestFullscreen) { /* Safari */
      elem.webkitRequestFullscreen();
    } else if (elem.msRequestFullscreen) { /* IE11 */
      elem.msRequestFullscreen();
    }
    isFullscreen = true;
  }
  
  function exitFullscreen() {
    if (document.exitFullscreen) {
      document.exitFullscreen();
    } else if (document.webkitExitFullscreen) { /* Safari */
      document.webkitExitFullscreen();
    } else if (document.msExitFullscreen) { /* IE11 */
      document.msExitFullscreen();
    }
    isFullscreen = false;
  }
  
  function preventScroll(e) {
    e.preventDefault();
    return false;
  }
  
  // Fullscreen change detection
  document.addEventListener('fullscreenchange', handleFullscreenChange);
  document.addEventListener('webkitfullscreenchange', handleFullscreenChange);
  document.addEventListener('msfullscreenchange', handleFullscreenChange);
  
  function handleFullscreenChange() {
    isFullscreen = !!(
      document.fullscreenElement ||
      document.webkitFullscreenElement ||
      document.msFullscreenElement
    );
  }
});
</script>